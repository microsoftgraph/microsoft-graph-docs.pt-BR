---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: ef23704c01a7d1b6cd3a85ffcab1dc34ded0936d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879433"
---
# <a name="list-deleted-items"></a><span data-ttu-id="09039-103">Listar itens excluídos</span><span class="sxs-lookup"><span data-stu-id="09039-103">List deleted items</span></span>

> <span data-ttu-id="09039-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="09039-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09039-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="09039-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="09039-106">Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="09039-106">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="09039-107">Atualmente, a funcionalidade de itens excluídos apenas tem suporte para os recursos [group](../resources/group.md) e [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="09039-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="09039-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="09039-108">Permissions</span></span>
<span data-ttu-id="09039-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09039-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="09039-111">Para usuários: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09039-111">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="09039-112">Para grupos: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="09039-112">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="09039-113">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09039-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="09039-114">Essa API dá suporte atualmente à recuperação de tipos de objeto de grupos (microsoft.graph.group) ou usuários (microsoft.graph.user) de itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="09039-114">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="09039-115">O tipo é especificado como uma parte obrigatória do URI.</span><span class="sxs-lookup"><span data-stu-id="09039-115">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="09039-116">Não há suporte para a chamada de GET /directory/deleteditems sem um tipo.</span><span class="sxs-lookup"><span data-stu-id="09039-116">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="09039-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09039-117">Optional query parameters</span></span>
<span data-ttu-id="09039-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09039-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09039-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09039-119">Request headers</span></span>
| <span data-ttu-id="09039-120">Nome</span><span class="sxs-lookup"><span data-stu-id="09039-120">Name</span></span>      |<span data-ttu-id="09039-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="09039-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09039-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="09039-122">Authorization</span></span>  | <span data-ttu-id="09039-123">&lt;Código&gt; do portador *Obrigatório*</span><span class="sxs-lookup"><span data-stu-id="09039-123">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="09039-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09039-124">Accept</span></span>  | <span data-ttu-id="09039-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09039-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09039-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09039-126">Request body</span></span>
<span data-ttu-id="09039-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09039-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09039-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="09039-128">Response</span></span>

<span data-ttu-id="09039-129">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09039-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="09039-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09039-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09039-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09039-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="09039-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="09039-132">Response</span></span>
<span data-ttu-id="09039-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09039-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
