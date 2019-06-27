---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0e6e3d70e53908133f4b195d54d8bc0f429e9ef4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273091"
---
# <a name="get-deleted-item"></a><span data-ttu-id="e0854-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="e0854-103">Get deleted item</span></span>

<span data-ttu-id="e0854-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="e0854-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="e0854-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="e0854-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0854-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0854-106">Permissions</span></span>
<span data-ttu-id="e0854-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="e0854-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="e0854-109">For users:</span></span>

|<span data-ttu-id="e0854-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0854-110">Permission type</span></span>      | <span data-ttu-id="e0854-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0854-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0854-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0854-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e0854-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0854-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="e0854-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0854-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0854-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0854-115">Not supported.</span></span> |
|<span data-ttu-id="e0854-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0854-116">Application</span></span> | <span data-ttu-id="e0854-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0854-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="e0854-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="e0854-118">For groups:</span></span>

|<span data-ttu-id="e0854-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0854-119">Permission type</span></span>      | <span data-ttu-id="e0854-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0854-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0854-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0854-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e0854-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0854-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e0854-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0854-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0854-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0854-124">Not supported.</span></span>    |
|<span data-ttu-id="e0854-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0854-125">Application</span></span> | <span data-ttu-id="e0854-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0854-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0854-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0854-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0854-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0854-128">Optional query parameters</span></span>
<span data-ttu-id="e0854-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0854-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0854-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0854-130">Request headers</span></span>
| <span data-ttu-id="e0854-131">Nome</span><span class="sxs-lookup"><span data-stu-id="e0854-131">Name</span></span>      |<span data-ttu-id="e0854-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0854-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0854-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0854-133">Authorization</span></span>  | <span data-ttu-id="e0854-134">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="e0854-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e0854-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0854-135">Accept</span></span>  | <span data-ttu-id="e0854-136">application/json</span><span class="sxs-lookup"><span data-stu-id="e0854-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0854-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0854-137">Request body</span></span>
<span data-ttu-id="e0854-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0854-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0854-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0854-139">Response</span></span>

<span data-ttu-id="e0854-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0854-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0854-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0854-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0854-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0854-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="e0854-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0854-143">Response</span></span>
<span data-ttu-id="e0854-p102">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0854-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0854-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e0854-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0854-147">C#</span><span class="sxs-lookup"><span data-stu-id="e0854-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0854-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0854-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e0854-149">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="e0854-149">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directory-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
