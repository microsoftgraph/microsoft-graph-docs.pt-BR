---
title: Listar unifiedRoleAssignmentMultiple
description: Recupere as propriedades e os relacionamentos do objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7fc80e7246a706b3fce41d00f0f628444a9426ab
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160329"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="4ff9a-103">Listar unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="4ff9a-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="4ff9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ff9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff9a-105">Obtenha uma lista de objetos [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="4ff9a-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="4ff9a-106">Use isso para obter uma lista de atribuições de função no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-106">Use this to get a list of role assignments in Microsoft Intune.</span></span> <span data-ttu-id="4ff9a-107">Para outros aplicativos do Micrsoft 365 (como o Azure AD), use o [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4ff9a-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ff9a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ff9a-108">Permissions</span></span>

<span data-ttu-id="4ff9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ff9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ff9a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ff9a-111">Permission type</span></span> | <span data-ttu-id="4ff9a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ff9a-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="4ff9a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ff9a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4ff9a-114">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="4ff9a-114">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4ff9a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ff9a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ff9a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-116">Not supported.</span></span> |
| <span data-ttu-id="4ff9a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4ff9a-117">Application</span></span> | <span data-ttu-id="4ff9a-118">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4ff9a-118">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ff9a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ff9a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ff9a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4ff9a-120">Optional query parameters</span></span>

<span data-ttu-id="4ff9a-121">Essa operação requer o `$filter` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-121">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="4ff9a-122">Você pode filtrar as `roleDefinitionId` Propriedades ou `principalId` .</span><span class="sxs-lookup"><span data-stu-id="4ff9a-122">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="4ff9a-123">A `roleDefinitionId` propriedade pode ser uma ID de objeto role ou uma ID de objeto de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-123">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="4ff9a-124">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4ff9a-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ff9a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ff9a-125">Request headers</span></span>

| <span data-ttu-id="4ff9a-126">Nome</span><span class="sxs-lookup"><span data-stu-id="4ff9a-126">Name</span></span> | <span data-ttu-id="4ff9a-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ff9a-127">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="4ff9a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ff9a-128">Authorization</span></span> | <span data-ttu-id="4ff9a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ff9a-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ff9a-131">Request body</span></span>

<span data-ttu-id="4ff9a-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ff9a-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ff9a-133">Response</span></span>

<span data-ttu-id="4ff9a-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-134">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ff9a-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ff9a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ff9a-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ff9a-136">Request</span></span>

<span data-ttu-id="4ff9a-137">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="4ff9a-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ff9a-138">Response</span></span>

<span data-ttu-id="4ff9a-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-139">The following is an example of the response.</span></span>
> <span data-ttu-id="4ff9a-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4ff9a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
