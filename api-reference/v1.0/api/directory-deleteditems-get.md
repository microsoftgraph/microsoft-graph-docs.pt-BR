---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d84fe777cb5e99727dcf8168d03ff8f2ac25451
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656801"
---
# <a name="get-deleted-item"></a><span data-ttu-id="10bf2-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="10bf2-103">Get deleted item</span></span>

<span data-ttu-id="10bf2-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="10bf2-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="10bf2-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="10bf2-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="10bf2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="10bf2-106">Permissions</span></span>
<span data-ttu-id="10bf2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10bf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="10bf2-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="10bf2-109">For users:</span></span>

|<span data-ttu-id="10bf2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10bf2-110">Permission type</span></span>      | <span data-ttu-id="10bf2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10bf2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10bf2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10bf2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10bf2-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10bf2-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="10bf2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10bf2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10bf2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bf2-115">Not supported.</span></span> |
|<span data-ttu-id="10bf2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10bf2-116">Application</span></span> | <span data-ttu-id="10bf2-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bf2-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="10bf2-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="10bf2-118">For groups:</span></span>

|<span data-ttu-id="10bf2-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10bf2-119">Permission type</span></span>      | <span data-ttu-id="10bf2-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="10bf2-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10bf2-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10bf2-121">Delegated (work or school account)</span></span> | <span data-ttu-id="10bf2-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10bf2-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="10bf2-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10bf2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10bf2-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10bf2-124">Not supported.</span></span>    |
|<span data-ttu-id="10bf2-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10bf2-125">Application</span></span> | <span data-ttu-id="10bf2-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10bf2-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10bf2-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10bf2-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10bf2-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="10bf2-128">Optional query parameters</span></span>
<span data-ttu-id="10bf2-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="10bf2-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10bf2-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10bf2-130">Request headers</span></span>
| <span data-ttu-id="10bf2-131">Nome</span><span class="sxs-lookup"><span data-stu-id="10bf2-131">Name</span></span>      |<span data-ttu-id="10bf2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="10bf2-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="10bf2-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="10bf2-133">Authorization</span></span>  | <span data-ttu-id="10bf2-134">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="10bf2-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="10bf2-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10bf2-135">Accept</span></span>  | <span data-ttu-id="10bf2-136">application/json</span><span class="sxs-lookup"><span data-stu-id="10bf2-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="10bf2-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10bf2-137">Request body</span></span>
<span data-ttu-id="10bf2-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10bf2-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10bf2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bf2-139">Response</span></span>

<span data-ttu-id="10bf2-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10bf2-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10bf2-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10bf2-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10bf2-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10bf2-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="10bf2-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="10bf2-143">Response</span></span>
<span data-ttu-id="10bf2-p102">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10bf2-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="10bf2-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="10bf2-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="10bf2-147">C#</span><span class="sxs-lookup"><span data-stu-id="10bf2-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="10bf2-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="10bf2-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
