---
title: 'group: getMemberObjects'
description: 'Retornar todos os grupos e unidades administrativas dos quais o grupo é membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 91f7583ec2835083387dd549af64758aaf213568
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420256"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="17071-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="17071-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17071-106">Retornar todos os grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="17071-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="17071-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="17071-107">The check is transitive.</span></span> <span data-ttu-id="17071-108">Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="17071-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="17071-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="17071-109">Permissions</span></span>
<span data-ttu-id="17071-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17071-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17071-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17071-112">Permission type</span></span>      | <span data-ttu-id="17071-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17071-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17071-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17071-114">Delegated (work or school account)</span></span> | <span data-ttu-id="17071-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17071-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17071-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17071-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17071-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17071-117">Not supported.</span></span>    |
|<span data-ttu-id="17071-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17071-118">Application</span></span> | <span data-ttu-id="17071-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17071-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17071-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17071-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="17071-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17071-121">Request headers</span></span>
| <span data-ttu-id="17071-122">Nome</span><span class="sxs-lookup"><span data-stu-id="17071-122">Name</span></span>       | <span data-ttu-id="17071-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="17071-123">Type</span></span> | <span data-ttu-id="17071-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="17071-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17071-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="17071-125">Authorization</span></span>  | <span data-ttu-id="17071-126">string</span><span class="sxs-lookup"><span data-stu-id="17071-126">string</span></span>  | <span data-ttu-id="17071-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17071-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17071-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17071-129">Request body</span></span>
<span data-ttu-id="17071-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17071-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="17071-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="17071-131">Parameter</span></span>    | <span data-ttu-id="17071-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="17071-132">Type</span></span>   |<span data-ttu-id="17071-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="17071-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17071-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="17071-134">securityEnabledOnly</span></span>|<span data-ttu-id="17071-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="17071-135">Boolean</span></span>|<span data-ttu-id="17071-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="17071-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="17071-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="17071-138">Response</span></span>
<span data-ttu-id="17071-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="17071-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="17071-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17071-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="17071-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17071-141">Request</span></span>
<span data-ttu-id="17071-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="17071-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17071-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="17071-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17071-144">C#</span><span class="sxs-lookup"><span data-stu-id="17071-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17071-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17071-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17071-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="17071-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17071-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="17071-147">Response</span></span>
<span data-ttu-id="17071-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="17071-148">The following is an example of the response.</span></span>
><span data-ttu-id="17071-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17071-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "group: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
