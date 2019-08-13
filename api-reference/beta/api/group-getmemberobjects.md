---
title: 'group: getMemberObjects'
description: 'Retornar todos os grupos e unidades administrativas dos quais o grupo é membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 772b5967964d39bdee55abc2350a69bd233d709b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326342"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="4f040-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="4f040-105">group: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f040-106">Retornar todos os grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="4f040-106">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="4f040-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="4f040-107">The check is transitive.</span></span> <span data-ttu-id="4f040-108">Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="4f040-108">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f040-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="4f040-109">Permissions</span></span>
<span data-ttu-id="4f040-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f040-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f040-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f040-112">Permission type</span></span>      | <span data-ttu-id="4f040-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4f040-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f040-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f040-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4f040-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f040-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f040-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f040-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f040-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f040-117">Not supported.</span></span>    |
|<span data-ttu-id="4f040-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f040-118">Application</span></span> | <span data-ttu-id="4f040-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f040-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f040-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f040-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="4f040-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f040-121">Request headers</span></span>
| <span data-ttu-id="4f040-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4f040-122">Name</span></span>       | <span data-ttu-id="4f040-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f040-123">Type</span></span> | <span data-ttu-id="4f040-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f040-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4f040-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f040-125">Authorization</span></span>  | <span data-ttu-id="4f040-126">string</span><span class="sxs-lookup"><span data-stu-id="4f040-126">string</span></span>  | <span data-ttu-id="4f040-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f040-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f040-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f040-129">Request body</span></span>
<span data-ttu-id="4f040-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f040-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f040-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4f040-131">Parameter</span></span>    | <span data-ttu-id="4f040-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f040-132">Type</span></span>   |<span data-ttu-id="4f040-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f040-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f040-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4f040-134">securityEnabledOnly</span></span>|<span data-ttu-id="4f040-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f040-135">Boolean</span></span>|<span data-ttu-id="4f040-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="4f040-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="4f040-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f040-138">Response</span></span>
<span data-ttu-id="4f040-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="4f040-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="4f040-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f040-140">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4f040-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f040-141">Request</span></span>
<span data-ttu-id="4f040-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f040-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4f040-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f040-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4f040-144">C#</span><span class="sxs-lookup"><span data-stu-id="4f040-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f040-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f040-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4f040-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4f040-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4f040-147">Java</span><span class="sxs-lookup"><span data-stu-id="4f040-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4f040-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f040-148">Response</span></span>
<span data-ttu-id="4f040-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4f040-149">The following is an example of the response.</span></span>
><span data-ttu-id="4f040-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f040-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
