---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bf2ab96d2718fbfaea87ed89d8b859bccc36b747
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377068"
---
# <a name="get-directoryrole"></a><span data-ttu-id="7db46-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="7db46-103">Get directoryRole</span></span>

<span data-ttu-id="7db46-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7db46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7db46-105">Recupere as propriedades de um objeto [directoryRole](../resources/directoryrole.md) .</span><span class="sxs-lookup"><span data-stu-id="7db46-105">Retrieve the properties of a [directoryRole](../resources/directoryrole.md) object.</span></span> <span data-ttu-id="7db46-106">A função deve ser ativada no locatário para uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="7db46-106">The role must be activated in tenant for a successful response.</span></span>

> [!Note]
> <span data-ttu-id="7db46-107">Você pode usar a ID de objeto e a ID de modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="7db46-107">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="7db46-108">A ID de modelo de uma função interna é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="7db46-108">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="7db46-109">Para obter detalhes, consulte [role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="7db46-109">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="7db46-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="7db46-110">Permissions</span></span>
<span data-ttu-id="7db46-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7db46-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7db46-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7db46-113">Permission type</span></span>      | <span data-ttu-id="7db46-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7db46-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7db46-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7db46-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7db46-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="7db46-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7db46-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7db46-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7db46-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7db46-118">Not supported.</span></span>    |
|<span data-ttu-id="7db46-119">Application</span><span class="sxs-lookup"><span data-stu-id="7db46-119">Application</span></span> | <span data-ttu-id="7db46-120">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="7db46-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7db46-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7db46-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7db46-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7db46-122">Optional query parameters</span></span>
<span data-ttu-id="7db46-123">Esse método **não** tem suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, $filter não tem suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="7db46-123">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7db46-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7db46-124">Request headers</span></span>
| <span data-ttu-id="7db46-125">Nome</span><span class="sxs-lookup"><span data-stu-id="7db46-125">Name</span></span>       | <span data-ttu-id="7db46-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="7db46-126">Type</span></span> | <span data-ttu-id="7db46-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="7db46-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7db46-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="7db46-128">Authorization</span></span>  | <span data-ttu-id="7db46-129">string</span><span class="sxs-lookup"><span data-stu-id="7db46-129">string</span></span>  | <span data-ttu-id="7db46-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7db46-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7db46-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7db46-132">Request body</span></span>
<span data-ttu-id="7db46-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7db46-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7db46-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db46-134">Response</span></span>

<span data-ttu-id="7db46-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7db46-135">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="7db46-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7db46-136">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-objectid"></a><span data-ttu-id="7db46-137">Exemplo 1: obter a definição de uma função de diretório usando objectId</span><span class="sxs-lookup"><span data-stu-id="7db46-137">Example 1: Get the definition of a directory role using objectId</span></span>
##### <a name="request"></a><span data-ttu-id="7db46-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7db46-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7db46-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7db46-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_objectId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/23f3b4b4-8a29-4420-8052-e4950273bbda
```
# <a name="c"></a>[<span data-ttu-id="7db46-140">C#</span><span class="sxs-lookup"><span data-stu-id="7db46-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7db46-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7db46-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7db46-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7db46-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7db46-143">Java</span><span class="sxs-lookup"><span data-stu-id="7db46-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7db46-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db46-144">Response</span></span>
><span data-ttu-id="7db46-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7db46-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-the-definition-of-a-directory-role-using-templateid"></a><span data-ttu-id="7db46-146">Exemplo 2: obter a definição de uma função de diretório usando TemplateID</span><span class="sxs-lookup"><span data-stu-id="7db46-146">Example 2: Get the definition of a directory role using templateId</span></span>
##### <a name="request"></a><span data-ttu-id="7db46-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7db46-147">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf
```

##### <a name="response"></a><span data-ttu-id="7db46-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="7db46-148">Response</span></span>
><span data-ttu-id="7db46-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7db46-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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
