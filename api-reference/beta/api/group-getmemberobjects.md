---
title: 'group: getMemberObjects'
description: 'Retornar todos os grupos e unidades administrativas dos quais o grupo é membro. A verificação é transitiva. Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.'
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3e111ef7885f0e288d3b59356c791fca5081308e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42419860"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="0ec2d-105">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="0ec2d-105">group: getMemberObjects</span></span>

<span data-ttu-id="0ec2d-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ec2d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec2d-107">Retornar todos os grupos e unidades administrativas dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-107">Return all of the groups and administrative units that the group is a member of.</span></span> <span data-ttu-id="0ec2d-108">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-108">The check is transitive.</span></span> <span data-ttu-id="0ec2d-109">Observação: Grupos não podem ser membros de funções de diretório, então nenhuma função de diretório retornará.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-109">Note: Groups cannot be members of directory roles, so no directory roles will be returned.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ec2d-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ec2d-110">Permissions</span></span>
<span data-ttu-id="0ec2d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ec2d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ec2d-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ec2d-113">Permission type</span></span>      | <span data-ttu-id="0ec2d-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0ec2d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ec2d-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ec2d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="0ec2d-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ec2d-116">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ec2d-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ec2d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ec2d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-118">Not supported.</span></span>    |
|<span data-ttu-id="0ec2d-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ec2d-119">Application</span></span> | <span data-ttu-id="0ec2d-120">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ec2d-120">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ec2d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec2d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="0ec2d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec2d-122">Request headers</span></span>
| <span data-ttu-id="0ec2d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="0ec2d-123">Name</span></span>       | <span data-ttu-id="0ec2d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ec2d-124">Type</span></span> | <span data-ttu-id="0ec2d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec2d-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0ec2d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ec2d-126">Authorization</span></span>  | <span data-ttu-id="0ec2d-127">string</span><span class="sxs-lookup"><span data-stu-id="0ec2d-127">string</span></span>  | <span data-ttu-id="0ec2d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ec2d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec2d-130">Request body</span></span>
<span data-ttu-id="0ec2d-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0ec2d-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0ec2d-132">Parameter</span></span>    | <span data-ttu-id="0ec2d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ec2d-133">Type</span></span>   |<span data-ttu-id="0ec2d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec2d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ec2d-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="0ec2d-135">securityEnabledOnly</span></span>|<span data-ttu-id="0ec2d-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ec2d-136">Boolean</span></span>|<span data-ttu-id="0ec2d-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="0ec2d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec2d-139">Response</span></span>
<span data-ttu-id="0ec2d-140">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-140">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="0ec2d-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ec2d-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0ec2d-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ec2d-142">Request</span></span>
<span data-ttu-id="0ec2d-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ec2d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ec2d-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0ec2d-145">C#</span><span class="sxs-lookup"><span data-stu-id="0ec2d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ec2d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ec2d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ec2d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ec2d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0ec2d-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ec2d-148">Response</span></span>
<span data-ttu-id="0ec2d-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-149">The following is an example of the response.</span></span>
><span data-ttu-id="0ec2d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ec2d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
