---
title: Criar unifiedRoleAssignment
description: Criar um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 672eac457659c3af05f0a3e1fc92ec0fe283746e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454511"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="75a6d-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75a6d-103">Create unifiedRoleAssignment</span></span>

<span data-ttu-id="75a6d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="75a6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75a6d-105">Criar um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="75a6d-105">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="75a6d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="75a6d-106">Permissions</span></span>

<span data-ttu-id="75a6d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75a6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="75a6d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75a6d-109">Permission type</span></span>                        | <span data-ttu-id="75a6d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75a6d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="75a6d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75a6d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="75a6d-112">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="75a6d-112">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="75a6d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75a6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75a6d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75a6d-114">Not supported.</span></span> |
| <span data-ttu-id="75a6d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75a6d-115">Application</span></span>                            | <span data-ttu-id="75a6d-116">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="75a6d-116">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="75a6d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75a6d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="75a6d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75a6d-118">Request headers</span></span>

| <span data-ttu-id="75a6d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="75a6d-119">Name</span></span>          | <span data-ttu-id="75a6d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a6d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="75a6d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="75a6d-121">Authorization</span></span> | <span data-ttu-id="75a6d-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="75a6d-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="75a6d-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75a6d-123">Request body</span></span>

<span data-ttu-id="75a6d-124">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="75a6d-124">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="75a6d-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a6d-125">Response</span></span>

<span data-ttu-id="75a6d-126">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75a6d-126">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a6d-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75a6d-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="75a6d-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75a6d-128">Request</span></span>

<span data-ttu-id="75a6d-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="75a6d-129">The following is an example of the request.</span></span> <span data-ttu-id="75a6d-130">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="75a6d-130">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="75a6d-131">roleDefinitionId pode ser a ID de modelo de todo o serviço ou o roleDefinitionId específico do diretório.</span><span class="sxs-lookup"><span data-stu-id="75a6d-131">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>

# <a name="http"></a>[<span data-ttu-id="75a6d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="75a6d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_rbacapplication"
}-->

```http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-type: application/json

{ 
    "principalId":"a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "roleDefinitionId":"b0f54661-2d74-4c50-afa3-1ec803f12efe",
    "resourceScope":"/"
}
```
# <a name="c"></a>[<span data-ttu-id="75a6d-133">C#</span><span class="sxs-lookup"><span data-stu-id="75a6d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="75a6d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="75a6d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="75a6d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="75a6d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="75a6d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="75a6d-136">Response</span></span>

<span data-ttu-id="75a6d-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="75a6d-137">The following is an example of the response.</span></span>

> <span data-ttu-id="75a6d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75a6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "YUb1sHQtUEyvox7IA_Eu_mm3jqnUe4lEhvatluHVi2I-1",
    "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
    "resourceScope": "/",
    "roleDefinitionId": "b0f54661-2d74-4c50-afa3-1ec803f12efe"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
