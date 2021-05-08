---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: keylimesoda
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 51e74ec0dc6eee9fa21ef7b7843f088c378cfb31
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241069"
---
# <a name="list-deleted-items"></a><span data-ttu-id="a18ae-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="a18ae-103">List deleted items</span></span>

<span data-ttu-id="a18ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a18ae-105">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="a18ae-105">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="a18ae-106">Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.</span><span class="sxs-lookup"><span data-stu-id="a18ae-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="a18ae-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a18ae-107">Permissions</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

<span data-ttu-id="a18ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a18ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-applications"></a><span data-ttu-id="a18ae-110">Para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="a18ae-110">For applications:</span></span>

|<span data-ttu-id="a18ae-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a18ae-111">Permission type</span></span>      | <span data-ttu-id="a18ae-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a18ae-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18ae-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a18ae-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a18ae-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a18ae-114">Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a18ae-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a18ae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a18ae-116">Not supported.</span></span>    |
|<span data-ttu-id="a18ae-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a18ae-117">Application</span></span> | <span data-ttu-id="a18ae-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a18ae-118">Application.Read.All, Application.ReadWrite.All, Directory.Read.All</span></span> |

### <a name="for-users"></a><span data-ttu-id="a18ae-119">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="a18ae-119">For users:</span></span>

|<span data-ttu-id="a18ae-120">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a18ae-120">Permission type</span></span>      | <span data-ttu-id="a18ae-121">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a18ae-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18ae-122">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a18ae-122">Delegated (work or school account)</span></span> | <span data-ttu-id="a18ae-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a18ae-123">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a18ae-124">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a18ae-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18ae-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a18ae-125">Not supported.</span></span> |
|<span data-ttu-id="a18ae-126">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a18ae-126">Application</span></span> | <span data-ttu-id="a18ae-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18ae-127">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="a18ae-128">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="a18ae-128">For groups:</span></span>

|<span data-ttu-id="a18ae-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a18ae-129">Permission type</span></span>      | <span data-ttu-id="a18ae-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a18ae-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18ae-131">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a18ae-131">Delegated (work or school account)</span></span> | <span data-ttu-id="a18ae-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a18ae-132">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a18ae-133">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a18ae-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18ae-134">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a18ae-134">Not supported.</span></span>    |
|<span data-ttu-id="a18ae-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a18ae-135">Application</span></span> | <span data-ttu-id="a18ae-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a18ae-136">Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a18ae-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a18ae-137">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="a18ae-138">Essa API dá suporte atualmente à recuperação de tipos de objeto de grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="a18ae-138">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="a18ae-139">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="a18ae-139">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="a18ae-140">Não há suporte para chamar GET /directory/deletedItems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="a18ae-140">Calling GET /directory/deletedItems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a18ae-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a18ae-141">Optional query parameters</span></span>
<span data-ttu-id="a18ae-142">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a18ae-142">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a18ae-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a18ae-143">Request headers</span></span>
| <span data-ttu-id="a18ae-144">Nome</span><span class="sxs-lookup"><span data-stu-id="a18ae-144">Name</span></span>      |<span data-ttu-id="a18ae-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="a18ae-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a18ae-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="a18ae-146">Authorization</span></span>  | <span data-ttu-id="a18ae-147">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="a18ae-147">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="a18ae-148">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a18ae-148">Accept</span></span>  | <span data-ttu-id="a18ae-149">application/json</span><span class="sxs-lookup"><span data-stu-id="a18ae-149">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a18ae-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a18ae-150">Request body</span></span>
<span data-ttu-id="a18ae-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a18ae-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a18ae-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a18ae-152">Response</span></span>

<span data-ttu-id="a18ae-153">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a18ae-153">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a18ae-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a18ae-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="a18ae-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a18ae-155">Request</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```

### <a name="response"></a><span data-ttu-id="a18ae-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a18ae-156">Response</span></span>
<span data-ttu-id="a18ae-157">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a18ae-157">Note: The response object shown here might be shortened for readability.</span></span>
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
