---
title: Membros transitivos do grupo de lista
description: Obtenha uma lista dos membros do grupo.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 9116569521cb024cd6501e448f8dccad61f64260
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43396814"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="cda94-103">Membros transitivos do grupo de lista</span><span class="sxs-lookup"><span data-stu-id="cda94-103">List group transitive members</span></span>

<span data-ttu-id="cda94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cda94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cda94-105">Obtenha uma lista dos membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="cda94-105">Get a list of the group's members.</span></span> <span data-ttu-id="cda94-106">Um grupo pode ter usuários, contatos, dispositivos, entidades de serviço e outros grupos como membros.</span><span class="sxs-lookup"><span data-stu-id="cda94-106">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="cda94-107">Essa operação é transitiva e também retornará uma lista simples de todos os membros aninhados.</span><span class="sxs-lookup"><span data-stu-id="cda94-107">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="cda94-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="cda94-108">Permissions</span></span>

<span data-ttu-id="cda94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cda94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cda94-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cda94-111">Permission type</span></span>      | <span data-ttu-id="cda94-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cda94-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cda94-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cda94-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cda94-114">Directory. Read. All, Directory. AccessAsUser. All, User. ReadBasic. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="cda94-114">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="cda94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cda94-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cda94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cda94-116">Not supported.</span></span>    |
|<span data-ttu-id="cda94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cda94-117">Application</span></span> | <span data-ttu-id="cda94-118">Directory. Read. All, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="cda94-118">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="cda94-119">Observação: para listar os membros de um grupo de associação oculto, a permissão member. Read. Hidden é necessária.</span><span class="sxs-lookup"><span data-stu-id="cda94-119">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cda94-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cda94-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cda94-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cda94-121">Optional query parameters</span></span>

<span data-ttu-id="cda94-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cda94-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cda94-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cda94-123">Request headers</span></span>

| <span data-ttu-id="cda94-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cda94-124">Name</span></span>       | <span data-ttu-id="cda94-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="cda94-125">Type</span></span> | <span data-ttu-id="cda94-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cda94-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cda94-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cda94-127">Authorization</span></span>  | <span data-ttu-id="cda94-128">string</span><span class="sxs-lookup"><span data-stu-id="cda94-128">string</span></span>  | <span data-ttu-id="cda94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cda94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cda94-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cda94-131">Request body</span></span>

<span data-ttu-id="cda94-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cda94-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cda94-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cda94-133">Response</span></span>

<span data-ttu-id="cda94-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cda94-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cda94-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cda94-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="cda94-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cda94-136">Request</span></span>

<span data-ttu-id="cda94-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cda94-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cda94-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cda94-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```
# <a name="c"></a>[<span data-ttu-id="cda94-139">C#</span><span class="sxs-lookup"><span data-stu-id="cda94-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivemembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cda94-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cda94-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivemembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cda94-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cda94-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivemembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cda94-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cda94-142">Response</span></span>

<span data-ttu-id="cda94-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cda94-143">The following is an example of the response.</span></span>
><span data-ttu-id="cda94-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cda94-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cda94-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cda94-145">All the properties will be returned from an actual call.</span></span>
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
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
