---
title: 'group: getMemberObjects'
description: 'Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 99344b834ac1f7cfd3d0ed02a9bdfc91a23163e2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273546"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="5a4a4-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="5a4a4-105">group: getMemberObjects</span></span>
<span data-ttu-id="5a4a4-p102">Retorne todos os grupos dos quais este grupo é um membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-p102">Return all of the groups that this group is a member of. The check is transitive. Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a4a4-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a4a4-109">Permissions</span></span>
<span data-ttu-id="5a4a4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a4a4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a4a4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a4a4-112">Permission type</span></span>      | <span data-ttu-id="5a4a4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a4a4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a4a4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a4a4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5a4a4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5a4a4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5a4a4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a4a4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a4a4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-117">Not supported.</span></span>    |
|<span data-ttu-id="5a4a4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a4a4-118">Application</span></span> | <span data-ttu-id="5a4a4-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a4a4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a4a4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a4a4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="5a4a4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a4a4-121">Request headers</span></span>
| <span data-ttu-id="5a4a4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5a4a4-122">Name</span></span>       | <span data-ttu-id="5a4a4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a4a4-123">Type</span></span> | <span data-ttu-id="5a4a4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a4a4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a4a4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a4a4-125">Authorization</span></span>  | <span data-ttu-id="5a4a4-126">string</span><span class="sxs-lookup"><span data-stu-id="5a4a4-126">string</span></span>  | <span data-ttu-id="5a4a4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a4a4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a4a4-129">Request body</span></span>
<span data-ttu-id="5a4a4-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5a4a4-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5a4a4-131">Parameter</span></span>    | <span data-ttu-id="5a4a4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a4a4-132">Type</span></span>   |<span data-ttu-id="5a4a4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a4a4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a4a4-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="5a4a4-134">securityEnabledOnly</span></span>|<span data-ttu-id="5a4a4-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a4a4-135">Boolean</span></span>| <span data-ttu-id="5a4a4-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="5a4a4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a4a4-138">Response</span></span>
<span data-ttu-id="5a4a4-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="5a4a4-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a4a4-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="5a4a4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a4a4-141">Request</span></span>
<span data-ttu-id="5a4a4-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-142">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="5a4a4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a4a4-143">Response</span></span>
<span data-ttu-id="5a4a4-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-144">The following is an example of the response.</span></span>
><span data-ttu-id="5a4a4-145">**Observação:**  o objeto de resposta mostrado aqui pode ser encurtado por questões de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-145">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5a4a4-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a4a4-146">All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="5a4a4-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5a4a4-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5a4a4-148">C#</span><span class="sxs-lookup"><span data-stu-id="5a4a4-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a4a4-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="5a4a4-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_getmemberobjects-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5a4a4-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5a4a4-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_getmemberobjects-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
