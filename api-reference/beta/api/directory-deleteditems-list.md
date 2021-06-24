---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 213860aa7a5b93247b1e98de8da2ace8528cd111
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107645"
---
# <a name="list-deleted-items"></a><span data-ttu-id="23f16-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="23f16-103">List deleted items</span></span>

<span data-ttu-id="23f16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23f16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23f16-105">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="23f16-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="23f16-106">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="23f16-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="23f16-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="23f16-107">Permissions</span></span>

<span data-ttu-id="23f16-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23f16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="23f16-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="23f16-110">For applications:</span></span>

|<span data-ttu-id="23f16-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23f16-111">Permission type</span></span>      | <span data-ttu-id="23f16-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23f16-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f16-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23f16-113">Delegated (work or school account)</span></span> | <span data-ttu-id="23f16-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23f16-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="23f16-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23f16-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f16-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23f16-116">Not supported.</span></span>    |
|<span data-ttu-id="23f16-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23f16-117">Application</span></span> | <span data-ttu-id="23f16-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23f16-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="23f16-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="23f16-119">For users:</span></span>

|<span data-ttu-id="23f16-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23f16-120">Permission type</span></span>      | <span data-ttu-id="23f16-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23f16-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f16-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23f16-122">Delegated (work or school account)</span></span> | <span data-ttu-id="23f16-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23f16-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="23f16-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23f16-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f16-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23f16-125">Not supported.</span></span> |
|<span data-ttu-id="23f16-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23f16-126">Application</span></span> | <span data-ttu-id="23f16-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23f16-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="23f16-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="23f16-128">For groups:</span></span>

|<span data-ttu-id="23f16-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23f16-129">Permission type</span></span>      | <span data-ttu-id="23f16-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="23f16-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23f16-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23f16-131">Delegated (work or school account)</span></span> | <span data-ttu-id="23f16-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23f16-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="23f16-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23f16-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23f16-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23f16-134">Not supported.</span></span>    |
|<span data-ttu-id="23f16-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="23f16-135">Application</span></span> | <span data-ttu-id="23f16-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23f16-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23f16-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23f16-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="23f16-138">Atualmente, essa API dá suporte à recuperação de tipos de objeto de aplicativos (microsoft.graph.application), grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="23f16-138">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="23f16-139">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="23f16-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="23f16-140">Não há suporte para a chamada de GET /directory/deleteditems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="23f16-140">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="23f16-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="23f16-141">Optional query parameters</span></span>
<span data-ttu-id="23f16-142">Este método dá suporte ao `$orderBy` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="23f16-142">This method supports the `$orderBy` [OData query parameter](/graph/query-parameters) to help customize the response.</span></span> 

### <a name="examples-using-the-orderby-odata-query-parameter"></a><span data-ttu-id="23f16-143">Exemplos usando o parâmetro $orderBy consulta OData</span><span class="sxs-lookup"><span data-stu-id="23f16-143">Examples using the $orderBy OData query parameter</span></span>

<span data-ttu-id="23f16-144">O parâmetro de consulta OData é suportado nas propriedades `$orderBy` **deletedDateTime**, **displayName** e **userPrincipalName** dos tipos de objeto excluídos.</span><span class="sxs-lookup"><span data-stu-id="23f16-144">The `$orderBy` OData query parameter is supported on the **deletedDateTime**, **displayName**, and **userPrincipalName** properties of the deleted object types.</span></span> <span data-ttu-id="23f16-145">Na propriedade **deletedDateTime,** a consulta requer a adição dos parâmetros de consulta avançados ( Header **ConsistencyLevel** definido como e cadeia de [caracteres](/graph/aad-advanced-queries) `true` de `$count=true` consulta).</span><span class="sxs-lookup"><span data-stu-id="23f16-145">On the **deletedDateTime** property, the query requires adding the [advanced query parameters](/graph/aad-advanced-queries) (**ConsistencyLevel** header set to `true` and `$count=true` query string).</span></span>

| <span data-ttu-id="23f16-146">OData cast</span><span class="sxs-lookup"><span data-stu-id="23f16-146">OData cast</span></span> | <span data-ttu-id="23f16-147">Propriedades que suportam $orderBy</span><span class="sxs-lookup"><span data-stu-id="23f16-147">Properties supporting $orderBy</span></span> | <span data-ttu-id="23f16-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23f16-148">Example</span></span> |
| :--- | :--- | :--- |
| <span data-ttu-id="23f16-149">microsoft.graph.user</span><span class="sxs-lookup"><span data-stu-id="23f16-149">microsoft.graph.user</span></span> | <span data-ttu-id="23f16-150">deletedDateTime, displayName, userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23f16-150">deletedDateTime, displayName, userPrincipalName</span></span> | <span data-ttu-id="23f16-151">/directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23f16-151">/directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName</span></span> |
| <span data-ttu-id="23f16-152">microsoft.graph.group</span><span class="sxs-lookup"><span data-stu-id="23f16-152">microsoft.graph.group</span></span> | <span data-ttu-id="23f16-153">deletedDateTime, displayName</span><span class="sxs-lookup"><span data-stu-id="23f16-153">deletedDateTime, displayName</span></span> | <span data-ttu-id="23f16-154">/directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true</span><span class="sxs-lookup"><span data-stu-id="23f16-154">/directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true</span></span> |
| <span data-ttu-id="23f16-155">microsoft.graph.application</span><span class="sxs-lookup"><span data-stu-id="23f16-155">microsoft.graph.application</span></span> | <span data-ttu-id="23f16-156">deletedDateTime, displayName</span><span class="sxs-lookup"><span data-stu-id="23f16-156">deletedDateTime, displayName</span></span> | <span data-ttu-id="23f16-157">/directory/deletedItems/microsoft.graph.application?$orderBy=displayName</span><span class="sxs-lookup"><span data-stu-id="23f16-157">/directory/deletedItems/microsoft.graph.application?$orderBy=displayName</span></span> |
| <span data-ttu-id="23f16-158">microsoft.graph.device</span><span class="sxs-lookup"><span data-stu-id="23f16-158">microsoft.graph.device</span></span> | <span data-ttu-id="23f16-159">deletedDateTime, displayName</span><span class="sxs-lookup"><span data-stu-id="23f16-159">deletedDateTime, displayName</span></span> | <span data-ttu-id="23f16-160">/directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true</span><span class="sxs-lookup"><span data-stu-id="23f16-160">/directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true</span></span> |

## <a name="request-headers"></a><span data-ttu-id="23f16-161">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23f16-161">Request headers</span></span>
| <span data-ttu-id="23f16-162">Nome</span><span class="sxs-lookup"><span data-stu-id="23f16-162">Name</span></span>      |<span data-ttu-id="23f16-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="23f16-163">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="23f16-164">Autorização</span><span class="sxs-lookup"><span data-stu-id="23f16-164">Authorization</span></span>  | <span data-ttu-id="23f16-165">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="23f16-165">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="23f16-166">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23f16-166">Accept</span></span>  | <span data-ttu-id="23f16-167">application/json</span><span class="sxs-lookup"><span data-stu-id="23f16-167">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="23f16-168">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23f16-168">Request body</span></span>
<span data-ttu-id="23f16-169">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="23f16-169">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23f16-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f16-170">Response</span></span>

<span data-ttu-id="23f16-171">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23f16-171">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="23f16-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23f16-172">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23f16-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23f16-173">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="23f16-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="23f16-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="23f16-175">C#</span><span class="sxs-lookup"><span data-stu-id="23f16-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="23f16-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23f16-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="23f16-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23f16-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="23f16-178">Java</span><span class="sxs-lookup"><span data-stu-id="23f16-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="23f16-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="23f16-179">Response</span></span>
<span data-ttu-id="23f16-180">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="23f16-180">Note: The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
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
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
