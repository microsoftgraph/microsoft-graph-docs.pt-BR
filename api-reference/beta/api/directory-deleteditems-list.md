---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8c9aea77ca7f1fd088d1bfdb0efdb1fd5b86176c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435441"
---
# <a name="list-deleted-items"></a><span data-ttu-id="c4acd-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="c4acd-103">List deleted items</span></span>

<span data-ttu-id="c4acd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c4acd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4acd-105">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="c4acd-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="c4acd-106">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="c4acd-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4acd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4acd-107">Permissions</span></span>

<span data-ttu-id="c4acd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4acd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="c4acd-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="c4acd-110">For applications:</span></span>

|<span data-ttu-id="c4acd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4acd-111">Permission type</span></span>      | <span data-ttu-id="c4acd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4acd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4acd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4acd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c4acd-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4acd-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4acd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4acd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4acd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4acd-116">Not supported.</span></span>    |
|<span data-ttu-id="c4acd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4acd-117">Application</span></span> | <span data-ttu-id="c4acd-118">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4acd-118">Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="c4acd-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="c4acd-119">For users:</span></span>

|<span data-ttu-id="c4acd-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4acd-120">Permission type</span></span>      | <span data-ttu-id="c4acd-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4acd-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4acd-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4acd-122">Delegated (work or school account)</span></span> | <span data-ttu-id="c4acd-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4acd-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c4acd-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4acd-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4acd-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4acd-125">Not supported.</span></span> |
|<span data-ttu-id="c4acd-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4acd-126">Application</span></span> | <span data-ttu-id="c4acd-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4acd-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="c4acd-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="c4acd-128">For groups:</span></span>

|<span data-ttu-id="c4acd-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4acd-129">Permission type</span></span>      | <span data-ttu-id="c4acd-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4acd-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4acd-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4acd-131">Delegated (work or school account)</span></span> | <span data-ttu-id="c4acd-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4acd-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c4acd-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4acd-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4acd-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c4acd-134">Not supported.</span></span>    |
|<span data-ttu-id="c4acd-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4acd-135">Application</span></span> | <span data-ttu-id="c4acd-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4acd-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4acd-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4acd-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="c4acd-138">Atualmente, essa API oferece suporte à recuperação de tipos de objeto de aplicativos (Microsoft. Graph. Application), grupos (Microsoft. Graph. Group) ou usuários (Microsoft. Graph. User) dos itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="c4acd-138">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="c4acd-139">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="c4acd-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="c4acd-140">Não há suporte para a chamada de GET /directory/deleteditems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="c4acd-140">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c4acd-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4acd-141">Optional query parameters</span></span>
<span data-ttu-id="c4acd-142">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4acd-142">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4acd-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4acd-143">Request headers</span></span>
| <span data-ttu-id="c4acd-144">Nome</span><span class="sxs-lookup"><span data-stu-id="c4acd-144">Name</span></span>      |<span data-ttu-id="c4acd-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4acd-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4acd-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4acd-146">Authorization</span></span>  | <span data-ttu-id="c4acd-147">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="c4acd-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="c4acd-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c4acd-148">Accept</span></span>  | <span data-ttu-id="c4acd-149">application/json</span><span class="sxs-lookup"><span data-stu-id="c4acd-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4acd-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4acd-150">Request body</span></span>
<span data-ttu-id="c4acd-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4acd-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4acd-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4acd-152">Response</span></span>

<span data-ttu-id="c4acd-153">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4acd-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4acd-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4acd-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4acd-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4acd-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c4acd-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="c4acd-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="c"></a>[<span data-ttu-id="c4acd-157">C#</span><span class="sxs-lookup"><span data-stu-id="c4acd-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c4acd-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4acd-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c4acd-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c4acd-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c4acd-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4acd-160">Response</span></span>
<span data-ttu-id="c4acd-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4acd-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
