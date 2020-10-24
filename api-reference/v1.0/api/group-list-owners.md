---
title: Listar proprietários
description: 'Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f5190563b412fd5ae99c62a955981913acda1a0f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690249"
---
# <a name="list-owners"></a><span data-ttu-id="a1237-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="a1237-104">List owners</span></span>

<span data-ttu-id="a1237-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1237-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1237-106">Recupere uma lista dos proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1237-106">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="a1237-107">Os proprietários são um conjunto de usuários ou os diretores de serviço que têm permissão para modificar o objeto do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1237-107">The owners are a set of users or service principals who are allowed to modify the group object.</span></span> <span data-ttu-id="a1237-108">Os proprietários não estão atualmente disponíveis no Microsoft Graph para os grupos que foram criados no Exchange ou grupos que são sincronizados a partir de um ambiente no local.</span><span class="sxs-lookup"><span data-stu-id="a1237-108">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span>

><span data-ttu-id="a1237-109">**Observação:** No momento, as entidades de serviço não estão listadas como proprietários de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Microsoft Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="a1237-109">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1237-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1237-110">Permissions</span></span>
<span data-ttu-id="a1237-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1237-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1237-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1237-113">Permission type</span></span>      | <span data-ttu-id="a1237-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1237-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1237-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1237-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a1237-116">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1237-116">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span>   |
|<span data-ttu-id="a1237-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1237-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1237-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1237-118">Not supported.</span></span>    |
|<span data-ttu-id="a1237-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1237-119">Application</span></span> | <span data-ttu-id="a1237-120">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1237-120">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All, Group.Read.All and User.Read.All and Application.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a1237-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1237-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1237-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1237-122">Optional query parameters</span></span>
<span data-ttu-id="a1237-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1237-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1237-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1237-124">Request headers</span></span>
| <span data-ttu-id="a1237-125">Nome</span><span class="sxs-lookup"><span data-stu-id="a1237-125">Name</span></span>       | <span data-ttu-id="a1237-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1237-126">Type</span></span> | <span data-ttu-id="a1237-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1237-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a1237-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1237-128">Authorization</span></span>  | <span data-ttu-id="a1237-129">string</span><span class="sxs-lookup"><span data-stu-id="a1237-129">string</span></span>  | <span data-ttu-id="a1237-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1237-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a1237-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1237-132">Request body</span></span>
<span data-ttu-id="a1237-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1237-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1237-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1237-134">Response</span></span>
<span data-ttu-id="a1237-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1237-135">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1237-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1237-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a1237-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1237-137">Request</span></span>
<span data-ttu-id="a1237-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1237-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a1237-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="a1237-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="a1237-140">C#</span><span class="sxs-lookup"><span data-stu-id="a1237-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a1237-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a1237-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a1237-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a1237-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a1237-143">Java</span><span class="sxs-lookup"><span data-stu-id="a1237-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a1237-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1237-144">Response</span></span>
<span data-ttu-id="a1237-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1237-145">The following is an example of the response.</span></span>
><span data-ttu-id="a1237-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1237-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

