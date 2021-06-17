---
title: Listar membros
description: Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d90baace95b3698a84ef55f74cca327ab95b5081
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990859"
---
# <a name="list-members"></a><span data-ttu-id="7703b-104">Listar membros</span><span class="sxs-lookup"><span data-stu-id="7703b-104">List members</span></span>

<span data-ttu-id="7703b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7703b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7703b-p102">Recupera uma lista dos usuários atribuídos à função de diretório.  Somente usuários podem ser atribuídos a uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7703b-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>

<span data-ttu-id="7703b-108">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="7703b-108">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="7703b-109">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7703b-109">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="7703b-110">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="7703b-110">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="7703b-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="7703b-111">Permissions</span></span>
<span data-ttu-id="7703b-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7703b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7703b-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7703b-114">Permission type</span></span>      | <span data-ttu-id="7703b-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7703b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7703b-116">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7703b-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7703b-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7703b-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7703b-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7703b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7703b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7703b-119">Not supported.</span></span>    |
|<span data-ttu-id="7703b-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7703b-120">Application</span></span> | <span data-ttu-id="7703b-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7703b-121">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="7703b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7703b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-objectId}/members
GET /directoryRoles/roleTemplateId={role-templateId}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7703b-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7703b-123">Optional query parameters</span></span>
<span data-ttu-id="7703b-124">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7703b-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7703b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7703b-125">Request headers</span></span>
| <span data-ttu-id="7703b-126">Nome</span><span class="sxs-lookup"><span data-stu-id="7703b-126">Name</span></span>       | <span data-ttu-id="7703b-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7703b-127">Type</span></span> | <span data-ttu-id="7703b-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7703b-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7703b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7703b-129">Authorization</span></span>  | <span data-ttu-id="7703b-130">string</span><span class="sxs-lookup"><span data-stu-id="7703b-130">string</span></span>  | <span data-ttu-id="7703b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7703b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7703b-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7703b-133">Request body</span></span>
<span data-ttu-id="7703b-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7703b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7703b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7703b-135">Response</span></span>

<span data-ttu-id="7703b-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7703b-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7703b-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7703b-137">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-role-objectid"></a><span data-ttu-id="7703b-138">Exemplo 1: Obter os membros de uma função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="7703b-138">Example 1: Get the members of a directory role using role objectId</span></span>

#### <a name="request"></a><span data-ttu-id="7703b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7703b-139">Request</span></span>
<span data-ttu-id="7703b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7703b-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7703b-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="7703b-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="7703b-142">C#</span><span class="sxs-lookup"><span data-stu-id="7703b-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7703b-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7703b-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7703b-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7703b-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7703b-145">Java</span><span class="sxs-lookup"><span data-stu-id="7703b-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7703b-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="7703b-146">Response</span></span>
> <span data-ttu-id="7703b-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7703b-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

### <a name="example-2-get-the-members-of-a-directory-role-using-role-templateid"></a><span data-ttu-id="7703b-148">Exemplo 2: Obter os membros de uma função de diretório usando role templateId</span><span class="sxs-lookup"><span data-stu-id="7703b-148">Example 2: Get the members of a directory role using role templateId</span></span>

#### <a name="request"></a><span data-ttu-id="7703b-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7703b-149">Request</span></span>
<span data-ttu-id="7703b-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7703b-150">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7703b-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="7703b-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="7703b-152">C#</span><span class="sxs-lookup"><span data-stu-id="7703b-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7703b-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7703b-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7703b-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7703b-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7703b-155">Java</span><span class="sxs-lookup"><span data-stu-id="7703b-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7703b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="7703b-156">Response</span></span>
><span data-ttu-id="7703b-157">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7703b-157">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"Adele Vance",
      "givenName":"Adele",
      "jobTitle":null,
      "mail":"AdeleV@contoso.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Vance",
      "userPrincipalName":"AdeleV@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
