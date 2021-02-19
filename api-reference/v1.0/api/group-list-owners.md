---
title: Listar proprietários
description: 'Recupere uma lista de proprietários do grupo. Os proprietários são um conjunto de usuários que não são administradores e que têm permissão para alterar o objeto de grupo. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 40782e513791ddb2da19250c65b016564d36fd7e
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272202"
---
# <a name="list-owners"></a><span data-ttu-id="0793e-104">Listar proprietários</span><span class="sxs-lookup"><span data-stu-id="0793e-104">List owners</span></span>

<span data-ttu-id="0793e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0793e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0793e-106">Recupere uma lista dos proprietários do grupo.</span><span class="sxs-lookup"><span data-stu-id="0793e-106">Retrieve a list of the group's owners.</span></span> <span data-ttu-id="0793e-107">Os proprietários são um conjunto de usuários ou os diretores de serviço que têm permissão para modificar o objeto do grupo.</span><span class="sxs-lookup"><span data-stu-id="0793e-107">The owners are a set of users or service principals who are allowed to modify the group object.</span></span> <span data-ttu-id="0793e-108">Os proprietários não estão atualmente disponíveis no Microsoft Graph para os grupos que foram criados no Exchange ou grupos que são sincronizados a partir de um ambiente no local.</span><span class="sxs-lookup"><span data-stu-id="0793e-108">Owners are currently not available in Microsoft Graph for groups that were created in Exchange or groups that are synchronized from an on-premises environment.</span></span>

><span data-ttu-id="0793e-109">**Observação:** No momento, as entidades de serviço não estão listadas como proprietários de grupo devido à distribuição em estágios das entidades de serviço para o ponto de extremidade do Microsoft Graph v 1.0.</span><span class="sxs-lookup"><span data-stu-id="0793e-109">**Note:** Currently, service principals are not listed as group owners due to the staged rollout of service principals to the Microsoft Graph v1.0 endpoint.</span></span>

## <a name="permissions"></a><span data-ttu-id="0793e-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0793e-110">Permissions</span></span>
<span data-ttu-id="0793e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0793e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0793e-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0793e-113">Permission type</span></span>      | <span data-ttu-id="0793e-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0793e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0793e-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0793e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0793e-116">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0793e-116">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0793e-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0793e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0793e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0793e-118">Not supported.</span></span>    |
|<span data-ttu-id="0793e-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0793e-119">Application</span></span> | <span data-ttu-id="0793e-120">GroupMember.Read.All, Group.Read.All, Group.Member.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0793e-120">GroupMember.Read.All, Group.Read.All, GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>  |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0793e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0793e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0793e-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0793e-122">Optional query parameters</span></span>
<span data-ttu-id="0793e-123">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0793e-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0793e-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0793e-124">Request headers</span></span>
| <span data-ttu-id="0793e-125">Nome</span><span class="sxs-lookup"><span data-stu-id="0793e-125">Name</span></span>       | <span data-ttu-id="0793e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0793e-126">Type</span></span> | <span data-ttu-id="0793e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0793e-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0793e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="0793e-128">Authorization</span></span>  | <span data-ttu-id="0793e-129">string</span><span class="sxs-lookup"><span data-stu-id="0793e-129">string</span></span>  | <span data-ttu-id="0793e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0793e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0793e-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0793e-132">Request body</span></span>
<span data-ttu-id="0793e-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0793e-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0793e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0793e-134">Response</span></span>
<span data-ttu-id="0793e-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [user](../resources/user.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0793e-135">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0793e-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0793e-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0793e-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0793e-137">Request</span></span>
<span data-ttu-id="0793e-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0793e-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0793e-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="0793e-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_owners"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```
# <a name="c"></a>[<span data-ttu-id="0793e-140">C#</span><span class="sxs-lookup"><span data-stu-id="0793e-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-owners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0793e-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0793e-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-owners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0793e-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0793e-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-owners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0793e-143">Java</span><span class="sxs-lookup"><span data-stu-id="0793e-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-owners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0793e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="0793e-144">Response</span></span>
<span data-ttu-id="0793e-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0793e-145">The following is an example of the response.</span></span>
><span data-ttu-id="0793e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0793e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

