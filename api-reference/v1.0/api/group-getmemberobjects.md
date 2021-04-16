---
title: 'group: getMemberObjects'
description: Retorne todos os grupos dos quais este grupo é um membro.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 697ea12958a6bb206635726a2d0e18649db71378
ms.sourcegitcommit: 3eb37e0621540bee91f42a7c2d8457310e90f8b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869838"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="60da0-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="60da0-103">group: getMemberObjects</span></span>

<span data-ttu-id="60da0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60da0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60da0-p101">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="60da0-p101">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="60da0-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="60da0-108">Permissions</span></span>
<span data-ttu-id="60da0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60da0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60da0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60da0-111">Permission type</span></span>      | <span data-ttu-id="60da0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="60da0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60da0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60da0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="60da0-114">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="60da0-114">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="60da0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60da0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60da0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60da0-116">Not supported.</span></span>    |
|<span data-ttu-id="60da0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60da0-117">Application</span></span> | <span data-ttu-id="60da0-118">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60da0-118">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60da0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60da0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="60da0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60da0-120">Request headers</span></span>
| <span data-ttu-id="60da0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="60da0-121">Name</span></span>       | <span data-ttu-id="60da0-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="60da0-122">Type</span></span> | <span data-ttu-id="60da0-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="60da0-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60da0-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="60da0-124">Authorization</span></span>  | <span data-ttu-id="60da0-125">string</span><span class="sxs-lookup"><span data-stu-id="60da0-125">string</span></span>  | <span data-ttu-id="60da0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60da0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60da0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60da0-128">Request body</span></span>
<span data-ttu-id="60da0-129">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60da0-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="60da0-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="60da0-130">Parameter</span></span>    | <span data-ttu-id="60da0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="60da0-131">Type</span></span>   |<span data-ttu-id="60da0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="60da0-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60da0-133">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="60da0-133">securityEnabledOnly</span></span>|<span data-ttu-id="60da0-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="60da0-134">Boolean</span></span>| <span data-ttu-id="60da0-p104">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="60da0-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="60da0-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="60da0-137">Response</span></span>
<span data-ttu-id="60da0-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="60da0-138">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="60da0-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60da0-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="60da0-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60da0-140">Request</span></span>
<span data-ttu-id="60da0-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="60da0-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="60da0-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="60da0-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="c"></a>[<span data-ttu-id="60da0-143">C#</span><span class="sxs-lookup"><span data-stu-id="60da0-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="60da0-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60da0-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="60da0-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60da0-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="60da0-146">Java</span><span class="sxs-lookup"><span data-stu-id="60da0-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="60da0-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="60da0-147">Response</span></span>
<span data-ttu-id="60da0-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="60da0-148">The following is an example of the response.</span></span>
><span data-ttu-id="60da0-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60da0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

