---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 368503c10b809571dcef4cef5265a86a37044031
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522708"
---
# <a name="get-directoryrole"></a><span data-ttu-id="2050b-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="2050b-103">Get directoryRole</span></span>

<span data-ttu-id="2050b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2050b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2050b-105">Recupere as propriedades de um objeto [directoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="2050b-105">Retrieve the properties of a [directoryRole](../resources/directoryrole.md) object.</span></span> <span data-ttu-id="2050b-106">A função deve ser ativada no locatário para uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="2050b-106">The role must be activated in tenant for a successful response.</span></span>

> [!Note]
> <span data-ttu-id="2050b-107">Você pode usar a ID de objeto e a ID de modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="2050b-107">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="2050b-108">A ID de modelo de uma função interna é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2050b-108">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="2050b-109">Para obter detalhes, consulte [role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="2050b-109">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="2050b-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="2050b-110">Permissions</span></span>
<span data-ttu-id="2050b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2050b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2050b-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2050b-113">Permission type</span></span>      | <span data-ttu-id="2050b-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2050b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2050b-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2050b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2050b-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="2050b-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2050b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2050b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2050b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2050b-118">Not supported.</span></span>    |
|<span data-ttu-id="2050b-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2050b-119">Application</span></span> | <span data-ttu-id="2050b-120">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2050b-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2050b-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2050b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2050b-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2050b-122">Optional query parameters</span></span>
<span data-ttu-id="2050b-123">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="2050b-123">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2050b-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2050b-124">Request headers</span></span>
| <span data-ttu-id="2050b-125">Nome</span><span class="sxs-lookup"><span data-stu-id="2050b-125">Name</span></span>       | <span data-ttu-id="2050b-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="2050b-126">Type</span></span> | <span data-ttu-id="2050b-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2050b-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2050b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2050b-128">Authorization</span></span>  | <span data-ttu-id="2050b-129">string</span><span class="sxs-lookup"><span data-stu-id="2050b-129">string</span></span>  | <span data-ttu-id="2050b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2050b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2050b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2050b-132">Request body</span></span>
<span data-ttu-id="2050b-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2050b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2050b-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2050b-134">Response</span></span>

<span data-ttu-id="2050b-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2050b-135">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2050b-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2050b-136">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-objectid"></a><span data-ttu-id="2050b-137">Exemplo 1: obter a definição de uma função de diretório usando objectId</span><span class="sxs-lookup"><span data-stu-id="2050b-137">Example 1: Get the definition of a directory role using objectId</span></span>
##### <a name="request"></a><span data-ttu-id="2050b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2050b-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2050b-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2050b-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_objectId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda
```
# <a name="c"></a>[<span data-ttu-id="2050b-140">C#</span><span class="sxs-lookup"><span data-stu-id="2050b-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2050b-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2050b-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2050b-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2050b-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2050b-143">Java</span><span class="sxs-lookup"><span data-stu-id="2050b-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2050b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2050b-144">Response</span></span>
><span data-ttu-id="2050b-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2050b-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
    "id": "23f3b4b4-8a29-4420-8052-e4950273bbda",
    "deletedDateTime": null,
    "description": "Can read sign-in and audit reports.",
    "displayName": "Reports Reader",
    "roleTemplateId": "4a5d8f65-41da-4de4-8968-e035b65339cf"
}
```

### <a name="example-2-get-the-definition-of-a-directory-role-using-templateid"></a><span data-ttu-id="2050b-146">Exemplo 2: obter a definição de uma função de diretório usando TemplateID</span><span class="sxs-lookup"><span data-stu-id="2050b-146">Example 2: Get the definition of a directory role using templateId</span></span>
##### <a name="request"></a><span data-ttu-id="2050b-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2050b-147">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2050b-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="2050b-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf
```
# <a name="c"></a>[<span data-ttu-id="2050b-149">C#</span><span class="sxs-lookup"><span data-stu-id="2050b-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2050b-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2050b-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2050b-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2050b-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2050b-152">Java</span><span class="sxs-lookup"><span data-stu-id="2050b-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2050b-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="2050b-153">Response</span></span>
><span data-ttu-id="2050b-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2050b-154">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryRoles/$entity",
    "id": "23f3b4b4-8a29-4420-8052-e4950273bbda",
    "deletedDateTime": null,
    "description": "Allows ability to read usage reports.",
    "displayName": "Reports Reader",
    "roleTemplateId": "4a5d8f65-41da-4de4-8968-e035b65339cf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
