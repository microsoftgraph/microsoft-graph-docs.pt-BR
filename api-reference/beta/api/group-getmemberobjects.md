---
title: 'group: getMemberObjects'
description: 'Retornar todos os grupos e unidades administrativas dos quais o grupo é membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 73e976ab377ac74d0503e5b94891a6dc616e38fa
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539052"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="9c249-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="9c249-105">group: getMemberObjects</span></span>

<span data-ttu-id="9c249-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c249-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c249-107">Retornar todos os grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="9c249-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="9c249-108">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="9c249-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c249-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c249-109">Permissions</span></span>
<span data-ttu-id="9c249-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c249-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c249-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c249-112">Permission type</span></span>      | <span data-ttu-id="9c249-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c249-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c249-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c249-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9c249-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c249-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c249-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c249-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c249-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c249-117">Not supported.</span></span>    |
|<span data-ttu-id="9c249-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c249-118">Application</span></span> | <span data-ttu-id="9c249-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c249-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c249-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c249-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="9c249-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c249-121">Request headers</span></span>
| <span data-ttu-id="9c249-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9c249-122">Name</span></span>       | <span data-ttu-id="9c249-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c249-123">Type</span></span> | <span data-ttu-id="9c249-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c249-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c249-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c249-125">Authorization</span></span>  | <span data-ttu-id="9c249-126">string</span><span class="sxs-lookup"><span data-stu-id="9c249-126">string</span></span>  | <span data-ttu-id="9c249-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c249-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c249-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c249-129">Request body</span></span>
<span data-ttu-id="9c249-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c249-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9c249-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9c249-131">Parameter</span></span>    | <span data-ttu-id="9c249-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c249-132">Type</span></span>   |<span data-ttu-id="9c249-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c249-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c249-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="9c249-134">securityEnabledOnly</span></span>|<span data-ttu-id="9c249-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c249-135">Boolean</span></span>|<span data-ttu-id="9c249-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="9c249-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="9c249-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c249-138">Response</span></span>
<span data-ttu-id="9c249-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="9c249-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="9c249-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c249-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9c249-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c249-141">Request</span></span>
<span data-ttu-id="9c249-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c249-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c249-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c249-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="9c249-144">C#</span><span class="sxs-lookup"><span data-stu-id="9c249-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c249-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c249-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c249-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c249-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c249-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c249-147">Response</span></span>
<span data-ttu-id="9c249-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9c249-148">The following is an example of the response.</span></span>
><span data-ttu-id="9c249-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c249-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
