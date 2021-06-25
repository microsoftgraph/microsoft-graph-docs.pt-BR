---
title: Listar membros de uma função de diretório
description: Recupere a lista de entidades que são atribuídas à função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 51e9a1fec22df0abf326a21f1cd7309e343fc152
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118634"
---
# <a name="list-members-of-a-directory-role"></a><span data-ttu-id="6a5d0-103">Listar membros de uma função de diretório</span><span class="sxs-lookup"><span data-stu-id="6a5d0-103">List members of a directory role</span></span>

<span data-ttu-id="6a5d0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a5d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a5d0-105">Recupere a lista de entidades que são atribuídas à função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-105">Retrieve the list of principals that are assigned to the directory role.</span></span> 

<span data-ttu-id="6a5d0-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="6a5d0-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="6a5d0-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="6a5d0-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a5d0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a5d0-109">Permissions</span></span>
<span data-ttu-id="6a5d0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a5d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6a5d0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a5d0-112">Permission type</span></span>      | <span data-ttu-id="6a5d0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a5d0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a5d0-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a5d0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6a5d0-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a5d0-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a5d0-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a5d0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a5d0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-117">Not supported.</span></span>    |
|<span data-ttu-id="6a5d0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a5d0-118">Application</span></span> | <span data-ttu-id="6a5d0-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a5d0-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="6a5d0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a5d0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-id}/members
GET /directoryRoles/roleTemplateId={roleTemplateId}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a5d0-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6a5d0-121">Optional query parameters</span></span>
<span data-ttu-id="6a5d0-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6a5d0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a5d0-123">Request headers</span></span>
| <span data-ttu-id="6a5d0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6a5d0-124">Name</span></span>       | <span data-ttu-id="6a5d0-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a5d0-125">Type</span></span> | <span data-ttu-id="6a5d0-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a5d0-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a5d0-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a5d0-127">Authorization</span></span>  | <span data-ttu-id="6a5d0-128">string</span><span class="sxs-lookup"><span data-stu-id="6a5d0-128">string</span></span>  | <span data-ttu-id="6a5d0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a5d0-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a5d0-131">Request body</span></span>
<span data-ttu-id="6a5d0-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a5d0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a5d0-133">Response</span></span>

<span data-ttu-id="6a5d0-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="6a5d0-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a5d0-135">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-role-id"></a><span data-ttu-id="6a5d0-136">Exemplo 1: Obter os membros de uma função de diretório usando a id de função</span><span class="sxs-lookup"><span data-stu-id="6a5d0-136">Example 1: Get the members of a directory role using role id</span></span>

#### <a name="request"></a><span data-ttu-id="6a5d0-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a5d0-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a5d0-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a5d0-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="6a5d0-139">C#</span><span class="sxs-lookup"><span data-stu-id="6a5d0-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a5d0-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a5d0-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a5d0-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a5d0-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a5d0-142">Java</span><span class="sxs-lookup"><span data-stu-id="6a5d0-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6a5d0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a5d0-143">Response</span></span>
> <span data-ttu-id="6a5d0-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2-get-the-members-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="6a5d0-145">Exemplo 2: Obter os membros de uma função de diretório usando roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6a5d0-145">Example 2: Get the members of a directory role using roleTemplateId</span></span>

##### <a name="request"></a><span data-ttu-id="6a5d0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a5d0-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a5d0-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a5d0-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="6a5d0-148">C#</span><span class="sxs-lookup"><span data-stu-id="6a5d0-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a5d0-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a5d0-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a5d0-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a5d0-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a5d0-151">Java</span><span class="sxs-lookup"><span data-stu-id="6a5d0-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a5d0-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a5d0-152">Response</span></span>
><span data-ttu-id="6a5d0-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6a5d0-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
