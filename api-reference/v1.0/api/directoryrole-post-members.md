---
title: Adicionar membro da função de diretório
description: Use esta API para criar um novo membro de função de diretório.
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ae03863fd35d7438a5fa3b9ff2ae0bfa90e41dce
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854163"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="6142f-103">Adicionar membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="6142f-103">Add directory role member</span></span>

<span data-ttu-id="6142f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6142f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6142f-105">Crie um novo membro de função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6142f-105">Create a new directory role member.</span></span>

<span data-ttu-id="6142f-106">Você pode usar a ID do objeto e a ID do modelo do **directoryRole** com essa API.</span><span class="sxs-lookup"><span data-stu-id="6142f-106">You can use both the object ID and template ID of the **directoryRole** with this API.</span></span> <span data-ttu-id="6142f-107">A ID do modelo de uma função embutida é imutável e pode ser vista na descrição da função no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6142f-107">The template ID of a built-in role is immutable and can be seen in the role description on the Azure portal.</span></span> <span data-ttu-id="6142f-108">Para obter detalhes, consulte [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span><span class="sxs-lookup"><span data-stu-id="6142f-108">For details, see [Role template IDs](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#role-template-ids).</span></span>

## <a name="permissions"></a><span data-ttu-id="6142f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="6142f-109">Permissions</span></span>
<span data-ttu-id="6142f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6142f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6142f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6142f-112">Permission type</span></span>      | <span data-ttu-id="6142f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6142f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6142f-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6142f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6142f-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6142f-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6142f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6142f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6142f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6142f-117">Not supported.</span></span>    |
|<span data-ttu-id="6142f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6142f-118">Application</span></span> | <span data-ttu-id="6142f-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6142f-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="6142f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6142f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{role-objectId}/members/$ref
POST /directoryRoles/roleTemplateId={role-templateId}/members/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6142f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6142f-121">Request headers</span></span>
| <span data-ttu-id="6142f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6142f-122">Name</span></span>       | <span data-ttu-id="6142f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="6142f-123">Type</span></span> | <span data-ttu-id="6142f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6142f-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6142f-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6142f-125">Authorization</span></span>  | <span data-ttu-id="6142f-126">string</span><span class="sxs-lookup"><span data-stu-id="6142f-126">string</span></span>  | <span data-ttu-id="6142f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6142f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6142f-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6142f-129">Content-Type</span></span>  | <span data-ttu-id="6142f-130">string</span><span class="sxs-lookup"><span data-stu-id="6142f-130">string</span></span>  | <span data-ttu-id="6142f-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6142f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6142f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6142f-133">Request body</span></span>
<span data-ttu-id="6142f-134">No corpo da solicitação, forneça uma representação JSON de um objeto [directoryObject](../resources/directoryobject.md) ou [user](../resources/user.md) a ser adicionado.</span><span class="sxs-lookup"><span data-stu-id="6142f-134">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="6142f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6142f-135">Response</span></span>

<span data-ttu-id="6142f-136">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6142f-136">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6142f-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6142f-137">Examples</span></span>

### <a name="example-1-add-a-new-member-to-a-directory-role-using-role-objectid"></a><span data-ttu-id="6142f-138">Exemplo 1: Adicionar um novo membro a uma função de diretório usando objectId de função</span><span class="sxs-lookup"><span data-stu-id="6142f-138">Example 1: Add a new member to a directory role using role objectId</span></span>

<span data-ttu-id="6142f-139">Nesta solicitação, substitua pelo valor de id da função `fe8f10bf-c9c2-47eb-95cb-c26cc85f1830` de diretório que você deseja atribuir ao usuário ou objeto de  diretório.</span><span class="sxs-lookup"><span data-stu-id="6142f-139">In this request, replace `fe8f10bf-c9c2-47eb-95cb-c26cc85f1830` with the **id** value for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="6142f-140">Substitua `15c1a2d5-9101-44b2-83ab-885db8a647ca` pelo valor de **id** do seu objeto de diretório ou usuário.</span><span class="sxs-lookup"><span data-stu-id="6142f-140">Replace `15c1a2d5-9101-44b2-83ab-885db8a647ca` with the **id** value of your user or directory object.</span></span> 

##### <a name="request"></a><span data-ttu-id="6142f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6142f-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6142f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6142f-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_objectId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/fe8f10bf-c9c2-47eb-95cb-c26cc85f1830/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca"
}
```
# <a name="javascript"></a>[<span data-ttu-id="6142f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6142f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-objectid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6142f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6142f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-objectid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6142f-145">C#</span><span class="sxs-lookup"><span data-stu-id="6142f-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-objectid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6142f-146">Java</span><span class="sxs-lookup"><span data-stu-id="6142f-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-objectid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6142f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6142f-147">Response</span></span>
><span data-ttu-id="6142f-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6142f-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

### <a name="example-2-add-a-new-member-to-a-directory-role-using-role-templateid"></a><span data-ttu-id="6142f-149">Exemplo 2: Adicionar um novo membro a uma função de diretório usando role templateId</span><span class="sxs-lookup"><span data-stu-id="6142f-149">Example 2: Add a new member to a directory role using role templateId</span></span>

<span data-ttu-id="6142f-150">Nesta solicitação, substitua pelo valor da `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` **funçãoTemplateId** para a função de diretório que você deseja atribuir ao usuário ou objeto de diretório.</span><span class="sxs-lookup"><span data-stu-id="6142f-150">In this request, replace `88d8e3e3-8f55-4a1e-953a-9b9898b8876b` with the value of the **roleTemplateId** for the directory role you wish to assign to the user or directory object.</span></span> <span data-ttu-id="6142f-151">Substitua `bb165b45-151c-4cf6-9911-cd7188912848` pelo valor de **id** do seu objeto de diretório ou usuário.</span><span class="sxs-lookup"><span data-stu-id="6142f-151">Replace `bb165b45-151c-4cf6-9911-cd7188912848` with the **id** value of your user or directory object.</span></span> 

##### <a name="request"></a><span data-ttu-id="6142f-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6142f-152">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6142f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="6142f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole_templateId"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/roleTemplateId=88d8e3e3-8f55-4a1e-953a-9b9898b8876b/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/bb165b45-151c-4cf6-9911-cd7188912848"
}
```
# <a name="javascript"></a>[<span data-ttu-id="6142f-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6142f-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6142f-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6142f-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6142f-156">C#</span><span class="sxs-lookup"><span data-stu-id="6142f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6142f-157">Java</span><span class="sxs-lookup"><span data-stu-id="6142f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryobject-from-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6142f-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="6142f-158">Response</span></span>
><span data-ttu-id="6142f-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6142f-159">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

