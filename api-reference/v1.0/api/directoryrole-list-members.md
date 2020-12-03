---
title: Listar membros de uma função de diretório
description: Recupere a lista de entidades de segurança atribuídas à função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 357333bb1f15828e8dd4ee0d37233539ce47edbd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524559"
---
# <a name="list-members-of-a-directory-role"></a><span data-ttu-id="7cd3c-103">Listar membros de uma função de diretório</span><span class="sxs-lookup"><span data-stu-id="7cd3c-103">List members of a directory role</span></span>

<span data-ttu-id="7cd3c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cd3c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cd3c-105">Recupere a lista de entidades de segurança atribuídas à função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-105">Retrieve the list of principals that are assigned to the directory role.</span></span> 

> [!Note]
> <span data-ttu-id="7cd3c-106">Você pode usar a ID de objeto e a ID de modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="7cd3c-107">A ID de modelo de uma função interna é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="7cd3c-108">Para obter detalhes, consulte [role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="7cd3c-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cd3c-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="7cd3c-109">Permissions</span></span>
<span data-ttu-id="7cd3c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cd3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7cd3c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cd3c-112">Permission type</span></span>      | <span data-ttu-id="7cd3c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cd3c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cd3c-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cd3c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7cd3c-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="7cd3c-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7cd3c-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cd3c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cd3c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-117">Not supported.</span></span>    |
|<span data-ttu-id="7cd3c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cd3c-118">Application</span></span> | <span data-ttu-id="7cd3c-119">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7cd3c-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="7cd3c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd3c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7cd3c-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7cd3c-121">Optional query parameters</span></span>
<span data-ttu-id="7cd3c-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="7cd3c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd3c-123">Request headers</span></span>
| <span data-ttu-id="7cd3c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7cd3c-124">Name</span></span>       | <span data-ttu-id="7cd3c-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cd3c-125">Type</span></span> | <span data-ttu-id="7cd3c-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cd3c-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7cd3c-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cd3c-127">Authorization</span></span>  | <span data-ttu-id="7cd3c-128">string</span><span class="sxs-lookup"><span data-stu-id="7cd3c-128">string</span></span>  | <span data-ttu-id="7cd3c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cd3c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd3c-131">Request body</span></span>
<span data-ttu-id="7cd3c-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cd3c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd3c-133">Response</span></span>

<span data-ttu-id="7cd3c-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7cd3c-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7cd3c-135">Examples</span></span>

### <a name="example-1-get-the-members-of-a-directory-role-using-objectid"></a><span data-ttu-id="7cd3c-136">Exemplo 1: obter os membros de uma função de diretório usando objectId</span><span class="sxs-lookup"><span data-stu-id="7cd3c-136">Example 1: Get the members of a directory role using objectId</span></span>

##### <a name="request"></a><span data-ttu-id="7cd3c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd3c-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7cd3c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd3c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_objectid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda/members
```
# <a name="c"></a>[<span data-ttu-id="7cd3c-139">C#</span><span class="sxs-lookup"><span data-stu-id="7cd3c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cd3c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cd3c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cd3c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cd3c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cd3c-142">Java</span><span class="sxs-lookup"><span data-stu-id="7cd3c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7cd3c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd3c-143">Response</span></span>
> <span data-ttu-id="7cd3c-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```
### <a name="example-2-get-the-members-of-a-directory-role-using-templateid"></a><span data-ttu-id="7cd3c-145">Exemplo 2: obter os membros de uma função de diretório usando TemplateID</span><span class="sxs-lookup"><span data-stu-id="7cd3c-145">Example 2: Get the members of a directory role using templateId</span></span>

##### <a name="request"></a><span data-ttu-id="7cd3c-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cd3c-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7cd3c-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cd3c-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_members_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf/members
```
# <a name="c"></a>[<span data-ttu-id="7cd3c-148">C#</span><span class="sxs-lookup"><span data-stu-id="7cd3c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-members-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cd3c-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cd3c-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-members-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cd3c-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cd3c-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-members-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cd3c-151">Java</span><span class="sxs-lookup"><span data-stu-id="7cd3c-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-members-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7cd3c-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cd3c-152">Response</span></span>
><span data-ttu-id="7cd3c-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7cd3c-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
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
