---
title: Listar membros
description: Obtenha uma lista de membros de direto do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros.
localization_priority: Priority
ms.openlocfilehash: d7dfaede0e9deae6806499b504c6a58da2381ef5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833282"
---
# <a name="list-members"></a><span data-ttu-id="7dcd5-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="7dcd5-104">List members</span></span>
<span data-ttu-id="7dcd5-p102">Obtenha uma lista dos membros diretos do grupo. Um grupo pode ter usuários, contatos e outros grupos como membros. Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dcd5-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7dcd5-108">Permissions</span></span>
<span data-ttu-id="7dcd5-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7dcd5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dcd5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7dcd5-111">Permission type</span></span>      | <span data-ttu-id="7dcd5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7dcd5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dcd5-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7dcd5-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7dcd5-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dcd5-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="7dcd5-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7dcd5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dcd5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-116">Not supported.</span></span>    |
|<span data-ttu-id="7dcd5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7dcd5-117">Application</span></span> | <span data-ttu-id="7dcd5-118">User.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7dcd5-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dcd5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7dcd5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dcd5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7dcd5-120">Optional query parameters</span></span>
<span data-ttu-id="7dcd5-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dcd5-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcd5-122">Request headers</span></span>
| <span data-ttu-id="7dcd5-123">Nome</span><span class="sxs-lookup"><span data-stu-id="7dcd5-123">Name</span></span>       | <span data-ttu-id="7dcd5-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dcd5-124">Type</span></span> | <span data-ttu-id="7dcd5-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dcd5-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7dcd5-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7dcd5-126">Authorization</span></span>  | <span data-ttu-id="7dcd5-127">string</span><span class="sxs-lookup"><span data-stu-id="7dcd5-127">string</span></span>  | <span data-ttu-id="7dcd5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dcd5-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcd5-130">Request body</span></span>
<span data-ttu-id="7dcd5-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dcd5-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dcd5-132">Response</span></span>
<span data-ttu-id="7dcd5-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dcd5-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7dcd5-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7dcd5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7dcd5-135">Request</span></span>
<span data-ttu-id="7dcd5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="7dcd5-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7dcd5-137">Response</span></span>
<span data-ttu-id="7dcd5-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-138">The following is an example of the response.</span></span>
><span data-ttu-id="7dcd5-139">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dcd5-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7dcd5-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
