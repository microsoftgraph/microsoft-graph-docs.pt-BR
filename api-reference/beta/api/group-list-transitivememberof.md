---
title: Lista de grupos transitivos transitivos
description: Obter grupos e unidades administrativas dos quais o grupo é membro.  Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado. Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 58ed9365778ea6c29653d741a7e56cd0f0098bd4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420123"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="0ad6e-105">Lista de grupos transitivos transitivos</span><span class="sxs-lookup"><span data-stu-id="0ad6e-105">List group transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad6e-106">Obter grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-106">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="0ad6e-107">Essa operação é transitiva e também inclui todos os grupos dos quais esse grupo é um membro aninhado.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-107">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="0ad6e-108">Ao contrário de obter os grupos do Office 365 de um usuário, isso retorna todos os tipos de grupos, não apenas grupos do Office 365.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ad6e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ad6e-109">Permissions</span></span>

<span data-ttu-id="0ad6e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ad6e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ad6e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ad6e-112">Permission type</span></span>      | <span data-ttu-id="0ad6e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ad6e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ad6e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ad6e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0ad6e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ad6e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ad6e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ad6e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ad6e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-117">Not supported.</span></span>    |
|<span data-ttu-id="0ad6e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ad6e-118">Application</span></span> | <span data-ttu-id="0ad6e-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ad6e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ad6e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ad6e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ad6e-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ad6e-121">Optional query parameters</span></span>
<span data-ttu-id="0ad6e-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ad6e-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ad6e-123">Request headers</span></span>
| <span data-ttu-id="0ad6e-124">Nome</span><span class="sxs-lookup"><span data-stu-id="0ad6e-124">Name</span></span>       | <span data-ttu-id="0ad6e-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ad6e-125">Type</span></span> | <span data-ttu-id="0ad6e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ad6e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ad6e-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ad6e-127">Authorization</span></span>  | <span data-ttu-id="0ad6e-128">string</span><span class="sxs-lookup"><span data-stu-id="0ad6e-128">string</span></span>  | <span data-ttu-id="0ad6e-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ad6e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ad6e-131">Request body</span></span>
<span data-ttu-id="0ad6e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ad6e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ad6e-133">Response</span></span>
<span data-ttu-id="0ad6e-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ad6e-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ad6e-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ad6e-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ad6e-136">Request</span></span>
<span data-ttu-id="0ad6e-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0ad6e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ad6e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0ad6e-139">C#</span><span class="sxs-lookup"><span data-stu-id="0ad6e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ad6e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ad6e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0ad6e-141">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0ad6e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0ad6e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ad6e-142">Response</span></span>

<span data-ttu-id="0ad6e-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-143">The following is an example of the response.</span></span>
><span data-ttu-id="0ad6e-144">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-144">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0ad6e-145">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ad6e-145">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
