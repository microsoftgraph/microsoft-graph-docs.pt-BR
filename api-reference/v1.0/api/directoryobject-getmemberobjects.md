---
title: Obter objetos de membros
description: " Retorna todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. Esta função é transitiva. "
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6eec72fc6e9d502565000a68d3f957660855de27
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051477"
---
# <a name="get-member-objects"></a><span data-ttu-id="f4ddd-104">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="f4ddd-104">Get member objects</span></span>

<span data-ttu-id="f4ddd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4ddd-105">Namespace: microsoft.graph</span></span>

 <span data-ttu-id="f4ddd-p102">Retorna todos os grupos e funções de diretório dos quais o objeto de usuário, grupo ou diretório é membro. Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-p102">Returns all the groups and directory roles that a user, group, or directory object is a member of. This function is transitive.</span></span> 
 > <span data-ttu-id="f4ddd-108">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4ddd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="f4ddd-109">Permissions</span></span>
<span data-ttu-id="f4ddd-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4ddd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4ddd-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4ddd-112">Permission type</span></span>      | <span data-ttu-id="f4ddd-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4ddd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4ddd-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4ddd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4ddd-115">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4ddd-115">User.Read.All and Group.Read.All, Directory.Read.All</span></span>    |
|<span data-ttu-id="f4ddd-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4ddd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4ddd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-117">Not supported.</span></span>    |
|<span data-ttu-id="f4ddd-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4ddd-118">Application</span></span> | <span data-ttu-id="f4ddd-119">User.Read.All e Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4ddd-119">User.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4ddd-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4ddd-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="f4ddd-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ddd-121">Request headers</span></span>
| <span data-ttu-id="f4ddd-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f4ddd-122">Name</span></span>       | <span data-ttu-id="f4ddd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ddd-123">Type</span></span> | <span data-ttu-id="f4ddd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ddd-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4ddd-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4ddd-125">Authorization</span></span>  | <span data-ttu-id="f4ddd-126">string</span><span class="sxs-lookup"><span data-stu-id="f4ddd-126">string</span></span>  | <span data-ttu-id="f4ddd-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f4ddd-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f4ddd-129">Content-Type</span></span>   | <span data-ttu-id="f4ddd-130">string</span><span class="sxs-lookup"><span data-stu-id="f4ddd-130">string</span></span>  | <span data-ttu-id="f4ddd-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f4ddd-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f4ddd-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ddd-132">Request body</span></span>
<span data-ttu-id="f4ddd-133">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4ddd-134">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f4ddd-134">Parameter</span></span>    | <span data-ttu-id="f4ddd-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ddd-135">Type</span></span>   |<span data-ttu-id="f4ddd-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ddd-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4ddd-137">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f4ddd-137">securityEnabledOnly</span></span>|<span data-ttu-id="f4ddd-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4ddd-138">Boolean</span></span>| <span data-ttu-id="f4ddd-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="f4ddd-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4ddd-141">Response</span></span>

<span data-ttu-id="f4ddd-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-142">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4ddd-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4ddd-143">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f4ddd-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ddd-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f4ddd-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4ddd-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryObjects/{object-id}/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[<span data-ttu-id="f4ddd-146">C#</span><span class="sxs-lookup"><span data-stu-id="f4ddd-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4ddd-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4ddd-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4ddd-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4ddd-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4ddd-149">Java</span><span class="sxs-lookup"><span data-stu-id="f4ddd-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f4ddd-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4ddd-150">Response</span></span>
<span data-ttu-id="f4ddd-151">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f4ddd-151">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

