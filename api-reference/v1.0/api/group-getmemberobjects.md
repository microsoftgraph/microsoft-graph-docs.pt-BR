---
title: 'group: getMemberObjects'
description: Retorne todos os grupos dos quais este grupo é um membro.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: a5f71a53fba79da14674328760081a51fbdcea34
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030786"
---
# <a name="group-getmemberobjects"></a><span data-ttu-id="a6521-103">group: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a6521-103">group: getMemberObjects</span></span>

<span data-ttu-id="a6521-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6521-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a6521-105">Retorne todos os grupos dos quais este grupo é um membro.</span><span class="sxs-lookup"><span data-stu-id="a6521-105">Return all of the groups that this group is a member of.</span></span> <span data-ttu-id="a6521-106">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a6521-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6521-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6521-107">Permissions</span></span>
<span data-ttu-id="a6521-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6521-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6521-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6521-110">Permission type</span></span>      | <span data-ttu-id="a6521-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6521-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6521-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6521-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6521-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6521-113">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="a6521-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6521-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6521-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6521-115">Not supported.</span></span>    |
|<span data-ttu-id="a6521-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6521-116">Application</span></span> | <span data-ttu-id="a6521-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6521-117">Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6521-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6521-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/getMemberObjects
```

## <a name="request-headers"></a><span data-ttu-id="a6521-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6521-119">Request headers</span></span>
| <span data-ttu-id="a6521-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a6521-120">Name</span></span>       | <span data-ttu-id="a6521-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6521-121">Type</span></span> | <span data-ttu-id="a6521-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6521-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6521-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6521-123">Authorization</span></span>  | <span data-ttu-id="a6521-124">string</span><span class="sxs-lookup"><span data-stu-id="a6521-124">string</span></span>  | <span data-ttu-id="a6521-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6521-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6521-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6521-127">Request body</span></span>
<span data-ttu-id="a6521-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6521-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6521-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6521-129">Parameter</span></span>    | <span data-ttu-id="a6521-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6521-130">Type</span></span>   |<span data-ttu-id="a6521-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6521-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6521-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a6521-132">securityEnabledOnly</span></span>|<span data-ttu-id="a6521-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6521-133">Boolean</span></span>| <span data-ttu-id="a6521-p104">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="a6521-p104">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="a6521-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6521-136">Response</span></span>
<span data-ttu-id="a6521-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos dos quais o grupo é membro.</span><span class="sxs-lookup"><span data-stu-id="a6521-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a6521-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6521-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a6521-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6521-139">Request</span></span>
<span data-ttu-id="a6521-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6521-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6521-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6521-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a6521-142">C#</span><span class="sxs-lookup"><span data-stu-id="a6521-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6521-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6521-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6521-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6521-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6521-145">Java</span><span class="sxs-lookup"><span data-stu-id="a6521-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a6521-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6521-146">Response</span></span>
<span data-ttu-id="a6521-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6521-147">The following is an example of the response.</span></span>
><span data-ttu-id="a6521-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a6521-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

