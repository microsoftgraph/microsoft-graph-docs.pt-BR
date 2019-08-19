---
title: Criar unifiedRoleAssignment
description: Criar um novo objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 42a747377ab8e5ae21c87b0fe529e92028d1a013
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461265"
---
# <a name="create-unifiedroleassignment"></a><span data-ttu-id="087f6-103">Criar unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="087f6-103">Create unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="087f6-104">Criar um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="087f6-104">Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="087f6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="087f6-105">Permissions</span></span>

<span data-ttu-id="087f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="087f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="087f6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="087f6-108">Permission type</span></span>                        | <span data-ttu-id="087f6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="087f6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="087f6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="087f6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="087f6-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="087f6-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="087f6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="087f6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="087f6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="087f6-113">Not supported.</span></span> |
| <span data-ttu-id="087f6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="087f6-114">Application</span></span>                            | <span data-ttu-id="087f6-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="087f6-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="087f6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="087f6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /roleManagement/directory/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="087f6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="087f6-117">Request headers</span></span>

| <span data-ttu-id="087f6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="087f6-118">Name</span></span>          | <span data-ttu-id="087f6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="087f6-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="087f6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="087f6-120">Authorization</span></span> | <span data-ttu-id="087f6-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="087f6-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="087f6-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="087f6-122">Request body</span></span>

<span data-ttu-id="087f6-123">No corpo da solicitação, forneça uma representação JSON do objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="087f6-123">In the request body, supply a JSON representation of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="087f6-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="087f6-124">Response</span></span>

<span data-ttu-id="087f6-125">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="087f6-125">If successful, this method returns `201 Created` response code and a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="087f6-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="087f6-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="087f6-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="087f6-127">Request</span></span>

<span data-ttu-id="087f6-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="087f6-128">The following is an example of the request.</span></span> <span data-ttu-id="087f6-129">Observe o uso do roleTemplateId para roleDefinitionId.</span><span class="sxs-lookup"><span data-stu-id="087f6-129">Note the use of the roleTemplateId for roleDefinitionId.</span></span> <span data-ttu-id="087f6-130">roleDefinitionId pode ser a ID de modelo de todo o serviço ou o roleDefinitionId específico do diretório.</span><span class="sxs-lookup"><span data-stu-id="087f6-130">roleDefinitionId can be either the service-wide template Id or the directory-specific roleDefinitionId.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="087f6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="087f6-131">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="087f6-132">C#</span><span class="sxs-lookup"><span data-stu-id="087f6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-unifiedroleassignment-from-rbacapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="087f6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="087f6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-unifiedroleassignment-from-rbacapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="087f6-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="087f6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-unifiedroleassignment-from-rbacapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="087f6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="087f6-135">Response</span></span>

<span data-ttu-id="087f6-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="087f6-136">The following is an example of the response.</span></span>

> <span data-ttu-id="087f6-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="087f6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
