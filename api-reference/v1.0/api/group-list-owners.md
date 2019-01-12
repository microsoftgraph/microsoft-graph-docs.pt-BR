---
title: Listar proprietários
description: 'Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo. '
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5c8cf1c82ceab0a7fa2a7f78b6c229165448d46e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972205"
---
# <a name="list-owners"></a><span data-ttu-id="99676-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="99676-104">List owners</span></span>
<span data-ttu-id="99676-p102">Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo.</span><span class="sxs-lookup"><span data-stu-id="99676-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="99676-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="99676-107">Permissions</span></span>
<span data-ttu-id="99676-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99676-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99676-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99676-110">Permission type</span></span>      | <span data-ttu-id="99676-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="99676-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99676-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99676-112">Delegated (work or school account)</span></span> | <span data-ttu-id="99676-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99676-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="99676-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99676-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99676-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99676-115">Not supported.</span></span>    |
|<span data-ttu-id="99676-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99676-116">Application</span></span> | <span data-ttu-id="99676-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99676-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99676-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99676-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99676-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="99676-119">Optional query parameters</span></span>
<span data-ttu-id="99676-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="99676-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99676-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99676-121">Request headers</span></span>
| <span data-ttu-id="99676-122">Nome</span><span class="sxs-lookup"><span data-stu-id="99676-122">Name</span></span>       | <span data-ttu-id="99676-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="99676-123">Type</span></span> | <span data-ttu-id="99676-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="99676-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99676-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="99676-125">Authorization</span></span>  | <span data-ttu-id="99676-126">string</span><span class="sxs-lookup"><span data-stu-id="99676-126">string</span></span>  | <span data-ttu-id="99676-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99676-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99676-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99676-129">Request body</span></span>
<span data-ttu-id="99676-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="99676-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99676-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="99676-131">Response</span></span>
<span data-ttu-id="99676-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99676-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99676-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99676-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="99676-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99676-134">Request</span></span>
<span data-ttu-id="99676-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="99676-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="99676-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="99676-136">Response</span></span>
<span data-ttu-id="99676-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="99676-137">The following is an example of the response.</span></span>
><span data-ttu-id="99676-138">**Observação:** no objeto response mostrado aqui pode ser reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="99676-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="99676-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99676-139">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
