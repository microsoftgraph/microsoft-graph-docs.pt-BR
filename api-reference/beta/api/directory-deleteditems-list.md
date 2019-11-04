---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b6c0e92b0286f1efdddc962f478cfc277d08c493
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936850"
---
# <a name="list-deleted-items"></a><span data-ttu-id="aba70-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="aba70-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aba70-104">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="aba70-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="aba70-105">Atualmente, a funcionalidade de itens excluídos só é suportada para o [aplicativo](../resources/application.md), [grupo](../resources/group.md) e recursos do [usuário](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="aba70-105">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="aba70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="aba70-106">Permissions</span></span>
<span data-ttu-id="aba70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aba70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="aba70-109">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="aba70-109">For applications:</span></span>

|<span data-ttu-id="aba70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba70-110">Permission type</span></span>      | <span data-ttu-id="aba70-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aba70-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba70-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aba70-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aba70-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aba70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba70-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba70-115">Not supported.</span></span>    |
|<span data-ttu-id="aba70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba70-116">Application</span></span> | <span data-ttu-id="aba70-117">Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="aba70-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="aba70-118">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="aba70-118">For users:</span></span>

|<span data-ttu-id="aba70-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba70-119">Permission type</span></span>      | <span data-ttu-id="aba70-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aba70-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba70-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba70-121">Delegated (work or school account)</span></span> | <span data-ttu-id="aba70-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aba70-122">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="aba70-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba70-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba70-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba70-124">Not supported.</span></span> |
|<span data-ttu-id="aba70-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba70-125">Application</span></span> | <span data-ttu-id="aba70-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aba70-126">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="aba70-127">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="aba70-127">For groups:</span></span>

|<span data-ttu-id="aba70-128">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aba70-128">Permission type</span></span>      | <span data-ttu-id="aba70-129">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aba70-129">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aba70-130">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aba70-130">Delegated (work or school account)</span></span> | <span data-ttu-id="aba70-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aba70-131">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="aba70-132">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aba70-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aba70-133">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aba70-133">Not supported.</span></span>    |
|<span data-ttu-id="aba70-134">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aba70-134">Application</span></span> | <span data-ttu-id="aba70-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="aba70-135">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aba70-136">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aba70-136">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="aba70-137">Atualmente, essa API oferece suporte à recuperação de tipos de objeto de aplicativos (Microsoft. Graph. Application), grupos (Microsoft. Graph. Group) ou usuários (Microsoft. Graph. User) dos itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="aba70-137">This API currently supports retrieving object types of applications (microsoft.graph.application), groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="aba70-138">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="aba70-138">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="aba70-139">Não há suporte para a chamada de GET /directory/deleteditems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="aba70-139">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="aba70-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aba70-140">Optional query parameters</span></span>
<span data-ttu-id="aba70-141">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aba70-141">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aba70-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aba70-142">Request headers</span></span>
| <span data-ttu-id="aba70-143">Nome</span><span class="sxs-lookup"><span data-stu-id="aba70-143">Name</span></span>      |<span data-ttu-id="aba70-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="aba70-144">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aba70-145">Autorização</span><span class="sxs-lookup"><span data-stu-id="aba70-145">Authorization</span></span>  | <span data-ttu-id="aba70-146">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="aba70-146">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="aba70-147">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aba70-147">Accept</span></span>  | <span data-ttu-id="aba70-148">application/json</span><span class="sxs-lookup"><span data-stu-id="aba70-148">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="aba70-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aba70-149">Request body</span></span>
<span data-ttu-id="aba70-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aba70-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aba70-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba70-151">Response</span></span>

<span data-ttu-id="aba70-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aba70-152">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aba70-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aba70-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aba70-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aba70-154">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="aba70-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="aba70-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="aba70-156">C#</span><span class="sxs-lookup"><span data-stu-id="aba70-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aba70-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aba70-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="aba70-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aba70-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aba70-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="aba70-159">Response</span></span>
<span data-ttu-id="aba70-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aba70-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
