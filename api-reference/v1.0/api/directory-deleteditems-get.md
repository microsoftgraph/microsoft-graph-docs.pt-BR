---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: lleonard-msft
ms.openlocfilehash: e3a42fffba9a447661010ac9f6f5cff19df880c1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353708"
---
# <a name="get-deleted-item"></a><span data-ttu-id="ba294-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="ba294-103">Get deleted item</span></span>

<span data-ttu-id="ba294-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ba294-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ba294-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ba294-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba294-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba294-106">Permissions</span></span>
<span data-ttu-id="ba294-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="ba294-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="ba294-109">For users:</span></span>

|<span data-ttu-id="ba294-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba294-110">Permission type</span></span>      | <span data-ttu-id="ba294-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba294-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba294-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba294-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba294-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba294-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="ba294-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba294-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba294-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba294-115">Not supported.</span></span> |
|<span data-ttu-id="ba294-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba294-116">Application</span></span> | <span data-ttu-id="ba294-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba294-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="ba294-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="ba294-118">For groups:</span></span>

|<span data-ttu-id="ba294-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba294-119">Permission type</span></span>      | <span data-ttu-id="ba294-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba294-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba294-121">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba294-121">Delegated (work or school account)</span></span> | <span data-ttu-id="ba294-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ba294-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="ba294-123">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba294-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba294-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba294-124">Not supported.</span></span>    |
|<span data-ttu-id="ba294-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba294-125">Application</span></span> | <span data-ttu-id="ba294-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba294-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba294-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba294-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ba294-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ba294-128">Optional query parameters</span></span>
<span data-ttu-id="ba294-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ba294-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ba294-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba294-130">Request headers</span></span>
| <span data-ttu-id="ba294-131">Nome</span><span class="sxs-lookup"><span data-stu-id="ba294-131">Name</span></span>      |<span data-ttu-id="ba294-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba294-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ba294-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba294-133">Authorization</span></span>  | <span data-ttu-id="ba294-134">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="ba294-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ba294-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba294-135">Accept</span></span>  | <span data-ttu-id="ba294-136">application/json</span><span class="sxs-lookup"><span data-stu-id="ba294-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba294-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba294-137">Request body</span></span>
<span data-ttu-id="ba294-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba294-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba294-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba294-139">Response</span></span>

<span data-ttu-id="ba294-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba294-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ba294-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba294-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba294-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba294-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="ba294-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba294-143">Response</span></span>
<span data-ttu-id="ba294-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba294-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->