---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6b9df8782ac11daca16a5ffc0533839d46de3381
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937039"
---
# <a name="get-deleted-item"></a><span data-ttu-id="09b18-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="09b18-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09b18-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="09b18-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="09b18-105">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="09b18-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="09b18-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="09b18-106">Permissions</span></span>
<span data-ttu-id="09b18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09b18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="09b18-109">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="09b18-109">For applications:</span></span>

|<span data-ttu-id="09b18-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09b18-110">Permission type</span></span>      | <span data-ttu-id="09b18-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09b18-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09b18-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09b18-112">Delegated (work or school account)</span></span> | <span data-ttu-id="09b18-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09b18-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="09b18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09b18-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09b18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09b18-115">Not supported.</span></span>    |
|<span data-ttu-id="09b18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09b18-116">Application</span></span> | <span data-ttu-id="09b18-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="09b18-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="09b18-118">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="09b18-118">For users:</span></span>

|<span data-ttu-id="09b18-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09b18-119">Permission type</span></span>      | <span data-ttu-id="09b18-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09b18-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09b18-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09b18-121">Delegated (work or school account)</span></span> | <span data-ttu-id="09b18-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09b18-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="09b18-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09b18-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09b18-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09b18-124">Not supported.</span></span> |
|<span data-ttu-id="09b18-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09b18-125">Application</span></span> | <span data-ttu-id="09b18-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09b18-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="09b18-127">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="09b18-127">For groups:</span></span>

|<span data-ttu-id="09b18-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09b18-128">Permission type</span></span>      | <span data-ttu-id="09b18-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09b18-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="09b18-130">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09b18-130">Delegated (work or school account)</span></span> | <span data-ttu-id="09b18-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09b18-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="09b18-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09b18-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09b18-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09b18-133">Not supported.</span></span>    |
|<span data-ttu-id="09b18-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09b18-134">Application</span></span> | <span data-ttu-id="09b18-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09b18-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="09b18-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09b18-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09b18-137">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09b18-137">Optional query parameters</span></span>
<span data-ttu-id="09b18-138">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09b18-138">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09b18-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09b18-139">Request headers</span></span>
| <span data-ttu-id="09b18-140">Nome</span><span class="sxs-lookup"><span data-stu-id="09b18-140">Name</span></span>      |<span data-ttu-id="09b18-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="09b18-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09b18-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="09b18-142">Authorization</span></span>  | <span data-ttu-id="09b18-143">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="09b18-143">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="09b18-144">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09b18-144">Accept</span></span>  | <span data-ttu-id="09b18-145">application/json</span><span class="sxs-lookup"><span data-stu-id="09b18-145">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09b18-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09b18-146">Request body</span></span>
<span data-ttu-id="09b18-147">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09b18-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09b18-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="09b18-148">Response</span></span>

<span data-ttu-id="09b18-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09b18-149">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09b18-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09b18-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09b18-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09b18-151">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="09b18-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="09b18-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09b18-153">C#</span><span class="sxs-lookup"><span data-stu-id="09b18-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09b18-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09b18-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09b18-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="09b18-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="09b18-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="09b18-156">Response</span></span>
<span data-ttu-id="09b18-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09b18-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
