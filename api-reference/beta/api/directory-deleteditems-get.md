---
title: Obter item excluído
description: Recupera as propriedades de um item recentemente excluído em itens excluídos.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09996c27aec0183ded5b09b490c95fb95d57893a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926425"
---
# <a name="get-deleted-item"></a><span data-ttu-id="99ae4-103">Obter item excluído</span><span class="sxs-lookup"><span data-stu-id="99ae4-103">Get deleted item</span></span>

> <span data-ttu-id="99ae4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99ae4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99ae4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99ae4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99ae4-106">Recupera as propriedades de um item recentemente excluído em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="99ae4-106">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="99ae4-107">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="99ae4-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="99ae4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="99ae4-108">Permissions</span></span>
<span data-ttu-id="99ae4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99ae4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="99ae4-111">Para usuários: User.Read.All, User.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="99ae4-111">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="99ae4-112">Para grupos: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="99ae4-112">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="99ae4-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99ae4-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99ae4-114">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99ae4-114">Optional query parameters</span></span>
<span data-ttu-id="99ae4-115">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99ae4-115">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99ae4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99ae4-116">Request headers</span></span>
| <span data-ttu-id="99ae4-117">Nome</span><span class="sxs-lookup"><span data-stu-id="99ae4-117">Name</span></span>      |<span data-ttu-id="99ae4-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="99ae4-118">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99ae4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="99ae4-119">Authorization</span></span>  | <span data-ttu-id="99ae4-120">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="99ae4-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="99ae4-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99ae4-121">Accept</span></span>  | <span data-ttu-id="99ae4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="99ae4-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="99ae4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99ae4-123">Request body</span></span>
<span data-ttu-id="99ae4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99ae4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99ae4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="99ae4-125">Response</span></span>

<span data-ttu-id="99ae4-126">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99ae4-126">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="99ae4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99ae4-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99ae4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99ae4-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="99ae4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="99ae4-129">Response</span></span>
<span data-ttu-id="99ae4-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99ae4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
