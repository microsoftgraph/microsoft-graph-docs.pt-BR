---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2fb4bc8bd5b696da4c2b895255ebb41a5170ce4b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181768"
---
# <a name="list-deleted-items"></a><span data-ttu-id="36788-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="36788-103">List deleted items</span></span>

<span data-ttu-id="36788-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36788-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="36788-105">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="36788-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="36788-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="36788-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="36788-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="36788-107">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="36788-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36788-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="36788-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="36788-110">For applications:</span></span>

|<span data-ttu-id="36788-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36788-111">Permission type</span></span>      | <span data-ttu-id="36788-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36788-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36788-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36788-113">Delegated (work or school account)</span></span> | <span data-ttu-id="36788-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36788-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36788-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36788-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36788-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36788-116">Not supported.</span></span>    |
|<span data-ttu-id="36788-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36788-117">Application</span></span> | <span data-ttu-id="36788-118">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="36788-118">Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="36788-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="36788-119">For users:</span></span>

|<span data-ttu-id="36788-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36788-120">Permission type</span></span>      | <span data-ttu-id="36788-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36788-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36788-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36788-122">Delegated (work or school account)</span></span> | <span data-ttu-id="36788-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36788-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="36788-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36788-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36788-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36788-125">Not supported.</span></span> |
|<span data-ttu-id="36788-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36788-126">Application</span></span> | <span data-ttu-id="36788-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36788-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="36788-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="36788-128">For groups:</span></span>

|<span data-ttu-id="36788-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36788-129">Permission type</span></span>      | <span data-ttu-id="36788-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36788-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36788-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36788-131">Delegated (work or school account)</span></span> | <span data-ttu-id="36788-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36788-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="36788-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36788-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36788-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36788-134">Not supported.</span></span>    |
|<span data-ttu-id="36788-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36788-135">Application</span></span> | <span data-ttu-id="36788-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="36788-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36788-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36788-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="36788-138">Essa API dá suporte atualmente à recuperação de tipos de objeto de grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="36788-138">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="36788-139">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="36788-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="36788-140">Não há suporte para a chamada de GET/directory/deletedItems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="36788-140">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="36788-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36788-141">Optional query parameters</span></span>
<span data-ttu-id="36788-142">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36788-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36788-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36788-143">Request headers</span></span>
| <span data-ttu-id="36788-144">Nome</span><span class="sxs-lookup"><span data-stu-id="36788-144">Name</span></span>      |<span data-ttu-id="36788-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="36788-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36788-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="36788-146">Authorization</span></span>  | <span data-ttu-id="36788-147">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="36788-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="36788-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36788-148">Accept</span></span>  | <span data-ttu-id="36788-149">application/json</span><span class="sxs-lookup"><span data-stu-id="36788-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="36788-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36788-150">Request body</span></span>
<span data-ttu-id="36788-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36788-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36788-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="36788-152">Response</span></span>

<span data-ttu-id="36788-153">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36788-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36788-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36788-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36788-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36788-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="36788-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="36788-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="36788-157">C#</span><span class="sxs-lookup"><span data-stu-id="36788-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36788-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36788-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36788-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36788-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36788-160">Java</span><span class="sxs-lookup"><span data-stu-id="36788-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="36788-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="36788-161">Response</span></span>
<span data-ttu-id="36788-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36788-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
