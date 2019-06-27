---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 28e389aa03d085d8b0e28cfbb0a12646b6c99cd7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273021"
---
# <a name="list-deleted-items"></a><span data-ttu-id="8b48b-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="8b48b-103">List deleted items</span></span>

<span data-ttu-id="8b48b-104">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8b48b-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="8b48b-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="8b48b-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b48b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b48b-106">Permissions</span></span>
<span data-ttu-id="8b48b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b48b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="8b48b-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="8b48b-109">For users:</span></span>

|<span data-ttu-id="8b48b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b48b-110">Permission type</span></span>      | <span data-ttu-id="8b48b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b48b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b48b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b48b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b48b-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b48b-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8b48b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b48b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b48b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b48b-115">Not supported.</span></span> |
|<span data-ttu-id="8b48b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b48b-116">Application</span></span> | <span data-ttu-id="8b48b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b48b-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="8b48b-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="8b48b-118">For groups:</span></span>

|<span data-ttu-id="8b48b-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b48b-119">Permission type</span></span>      | <span data-ttu-id="8b48b-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b48b-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b48b-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b48b-121">Delegated (work or school account)</span></span> | <span data-ttu-id="8b48b-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8b48b-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="8b48b-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b48b-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b48b-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b48b-124">Not supported.</span></span>    |
|<span data-ttu-id="8b48b-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b48b-125">Application</span></span> | <span data-ttu-id="8b48b-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8b48b-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b48b-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b48b-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="8b48b-128">Essa API dá suporte atualmente à recuperação de tipos de objeto de grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="8b48b-128">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="8b48b-129">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="8b48b-129">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="8b48b-130">Não há suporte para a chamada de GET/directory/deletedItems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="8b48b-130">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8b48b-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b48b-131">Optional query parameters</span></span>
<span data-ttu-id="8b48b-132">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b48b-132">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b48b-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b48b-133">Request headers</span></span>
| <span data-ttu-id="8b48b-134">Nome</span><span class="sxs-lookup"><span data-stu-id="8b48b-134">Name</span></span>      |<span data-ttu-id="8b48b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b48b-135">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8b48b-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b48b-136">Authorization</span></span>  | <span data-ttu-id="8b48b-137">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="8b48b-137">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8b48b-138">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b48b-138">Accept</span></span>  | <span data-ttu-id="8b48b-139">application/json</span><span class="sxs-lookup"><span data-stu-id="8b48b-139">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b48b-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b48b-140">Request body</span></span>
<span data-ttu-id="8b48b-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b48b-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b48b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b48b-142">Response</span></span>

<span data-ttu-id="8b48b-143">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b48b-143">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b48b-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b48b-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b48b-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b48b-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="8b48b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b48b-146">Response</span></span>
<span data-ttu-id="8b48b-p103">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b48b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8b48b-149">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="8b48b-149">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8b48b-150">C#</span><span class="sxs-lookup"><span data-stu-id="8b48b-150">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_deleteditems-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b48b-151">Javascript</span><span class="sxs-lookup"><span data-stu-id="8b48b-151">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_deleteditems-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8b48b-152">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8b48b-152">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_deleteditems-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
