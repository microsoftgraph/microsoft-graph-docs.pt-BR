---
title: Obter directoryRole
description: Recupere as propriedades de um objeto directoryRole.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 997882a9385d9fa3c9f474b9d4fa6efc930af21f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991712"
---
# <a name="get-directoryrole"></a><span data-ttu-id="ffaa5-103">Obter directoryRole</span><span class="sxs-lookup"><span data-stu-id="ffaa5-103">Get directoryRole</span></span>

<span data-ttu-id="ffaa5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffaa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffaa5-105">Recupere as propriedades de um objeto directoryRole.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-105">Retrieve the properties of a directoryRole object.</span></span>

<span data-ttu-id="ffaa5-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="ffaa5-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="ffaa5-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="ffaa5-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="ffaa5-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="ffaa5-109">Permissions</span></span>
<span data-ttu-id="ffaa5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffaa5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffaa5-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ffaa5-112">Permission type</span></span>      | <span data-ttu-id="ffaa5-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ffaa5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffaa5-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ffaa5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ffaa5-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ffaa5-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ffaa5-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ffaa5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffaa5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-117">Not supported.</span></span>    |
|<span data-ttu-id="ffaa5-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ffaa5-118">Application</span></span> | <span data-ttu-id="ffaa5-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffaa5-119">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffaa5-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ffaa5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{role-objectId}
GET /directoryRoles/roleTemplateId={role-templateId}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffaa5-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ffaa5-121">Optional query parameters</span></span>
<span data-ttu-id="ffaa5-122">Esse método não **dá suporte** a [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta (por exemplo, `$filter` não há suporte aqui).</span><span class="sxs-lookup"><span data-stu-id="ffaa5-122">This method does **not** support any [OData Query Parameters](/graph/query-parameters) to help customize the response (for example, `$filter` is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffaa5-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaa5-123">Request headers</span></span>
| <span data-ttu-id="ffaa5-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ffaa5-124">Name</span></span>       | <span data-ttu-id="ffaa5-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="ffaa5-125">Type</span></span> | <span data-ttu-id="ffaa5-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ffaa5-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ffaa5-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="ffaa5-127">Authorization</span></span>  | <span data-ttu-id="ffaa5-128">string</span><span class="sxs-lookup"><span data-stu-id="ffaa5-128">string</span></span>  | <span data-ttu-id="ffaa5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffaa5-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaa5-131">Request body</span></span>
<span data-ttu-id="ffaa5-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffaa5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffaa5-133">Response</span></span>

<span data-ttu-id="ffaa5-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-134">If successful, this method returns a `200 OK` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="ffaa5-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ffaa5-135">Examples</span></span>

### <a name="example-1-get-the-definition-of-a-directory-role-using-role-objectid"></a><span data-ttu-id="ffaa5-136">Exemplo 1: Obter a definição de uma função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="ffaa5-136">Example 1: Get the definition of a directory role using role objectId</span></span>
#### <a name="request"></a><span data-ttu-id="ffaa5-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaa5-137">Request</span></span>
<span data-ttu-id="ffaa5-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ffaa5-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffaa5-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830
```
# <a name="c"></a>[<span data-ttu-id="ffaa5-140">C#</span><span class="sxs-lookup"><span data-stu-id="ffaa5-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffaa5-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffaa5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffaa5-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffaa5-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffaa5-143">Java</span><span class="sxs-lookup"><span data-stu-id="ffaa5-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="ffaa5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffaa5-144">Response</span></span>
><span data-ttu-id="ffaa5-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```


### <a name="example-2-get-the-definition-of-a-directory-role-using-role-templateid"></a><span data-ttu-id="ffaa5-146">Exemplo 2: Obter a definição de uma função de diretório usando role templateId</span><span class="sxs-lookup"><span data-stu-id="ffaa5-146">Example 2: Get the definition of a directory role using role templateId</span></span>
#### <a name="request"></a><span data-ttu-id="ffaa5-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ffaa5-147">Request</span></span>
<span data-ttu-id="ffaa5-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-148">Here is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="ffaa5-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffaa5-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b
```
# <a name="c"></a>[<span data-ttu-id="ffaa5-150">C#</span><span class="sxs-lookup"><span data-stu-id="ffaa5-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ffaa5-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffaa5-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ffaa5-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ffaa5-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ffaa5-153">Java</span><span class="sxs-lookup"><span data-stu-id="ffaa5-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ffaa5-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ffaa5-154">Response</span></span>
><span data-ttu-id="ffaa5-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ffaa5-155">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryRoles/$entity",
    "id": "fe8f10bf-c9c2-47eb-95cb-c26cc85f1830",
    "deletedDateTime": null,
    "description": "Can read basic directory information. Commonly used to grant directory read access to applications and guests.",
    "displayName": "Directory Readers",
    "roleTemplateId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
