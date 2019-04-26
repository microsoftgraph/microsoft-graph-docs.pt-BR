---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de025535058c8b796b591b5bcac2f91f4d3397e3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555091"
---
# <a name="get-deleted-item"></a><span data-ttu-id="1cc33-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="1cc33-103">Get deleted item</span></span>

<span data-ttu-id="1cc33-104">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="1cc33-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="1cc33-105">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="1cc33-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc33-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cc33-106">Permissions</span></span>
<span data-ttu-id="1cc33-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="1cc33-109">Para usuários:</span><span class="sxs-lookup"><span data-stu-id="1cc33-109">For users:</span></span>

|<span data-ttu-id="1cc33-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc33-110">Permission type</span></span>      | <span data-ttu-id="1cc33-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc33-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc33-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cc33-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="1cc33-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc33-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc33-115">Not supported.</span></span> |
|<span data-ttu-id="1cc33-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc33-116">Application</span></span> | <span data-ttu-id="1cc33-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc33-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="1cc33-118">Para grupos:</span><span class="sxs-lookup"><span data-stu-id="1cc33-118">For groups:</span></span>

|<span data-ttu-id="1cc33-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc33-119">Permission type</span></span>      | <span data-ttu-id="1cc33-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc33-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cc33-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc33-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1cc33-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cc33-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1cc33-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc33-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc33-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc33-124">Not supported.</span></span>    |
|<span data-ttu-id="1cc33-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc33-125">Application</span></span> | <span data-ttu-id="1cc33-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc33-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc33-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc33-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cc33-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1cc33-128">Optional query parameters</span></span>
<span data-ttu-id="1cc33-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc33-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cc33-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc33-130">Request headers</span></span>
| <span data-ttu-id="1cc33-131">Nome</span><span class="sxs-lookup"><span data-stu-id="1cc33-131">Name</span></span>      |<span data-ttu-id="1cc33-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc33-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1cc33-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cc33-133">Authorization</span></span>  | <span data-ttu-id="1cc33-134">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="1cc33-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="1cc33-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1cc33-135">Accept</span></span>  | <span data-ttu-id="1cc33-136">application/json</span><span class="sxs-lookup"><span data-stu-id="1cc33-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc33-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc33-137">Request body</span></span>
<span data-ttu-id="1cc33-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cc33-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cc33-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc33-139">Response</span></span>

<span data-ttu-id="1cc33-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc33-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1cc33-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cc33-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cc33-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc33-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
##### <a name="response"></a><span data-ttu-id="1cc33-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc33-143">Response</span></span>
<span data-ttu-id="1cc33-p102">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cc33-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
