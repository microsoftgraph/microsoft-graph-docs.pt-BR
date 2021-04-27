---
title: Listar UnifiedRoleAssignmentMultiple
description: Recupere as propriedades e as relações do objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 062cd1d5c39c64eab9018289127eb5c6e691bd44
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054753"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="3da26-103">Listar UnifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="3da26-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="3da26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3da26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3da26-105">Obter uma lista do [objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="3da26-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="3da26-106">Use isso para obter uma lista de atribuições de função Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="3da26-106">Use this to get a list of role assignments in Microsoft Intune.</span></span> <span data-ttu-id="3da26-107">Para outros Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3da26-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3da26-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3da26-108">Permissions</span></span>

<span data-ttu-id="3da26-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3da26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3da26-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3da26-111">Permission type</span></span> | <span data-ttu-id="3da26-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3da26-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="3da26-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3da26-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3da26-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da26-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="3da26-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3da26-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3da26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3da26-116">Not supported.</span></span> |
| <span data-ttu-id="3da26-117">Application</span><span class="sxs-lookup"><span data-stu-id="3da26-117">Application</span></span> | <span data-ttu-id="3da26-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3da26-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3da26-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3da26-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3da26-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3da26-120">Optional query parameters</span></span>
<span data-ttu-id="3da26-121">Você pode filtrar as `roleDefinitionId` propriedades `principalId` ou.</span><span class="sxs-lookup"><span data-stu-id="3da26-121">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="3da26-122">A propriedade pode ser uma ID de objeto de função ou uma ID de objeto `roleDefinitionId` de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="3da26-122">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="3da26-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3da26-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3da26-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3da26-124">Request headers</span></span>

| <span data-ttu-id="3da26-125">Nome</span><span class="sxs-lookup"><span data-stu-id="3da26-125">Name</span></span> | <span data-ttu-id="3da26-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="3da26-126">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="3da26-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="3da26-127">Authorization</span></span> | <span data-ttu-id="3da26-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3da26-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3da26-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3da26-130">Request body</span></span>

<span data-ttu-id="3da26-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3da26-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3da26-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da26-132">Response</span></span>

<span data-ttu-id="3da26-133">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3da26-133">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3da26-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3da26-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3da26-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3da26-135">Request</span></span>

<span data-ttu-id="3da26-136">Veja a seguir um exemplo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="3da26-136">The following is an example of the request:</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="3da26-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3da26-137">Response</span></span>

<span data-ttu-id="3da26-138">Veja a seguir um exemplo da resposta:</span><span class="sxs-lookup"><span data-stu-id="3da26-138">The following is an example of the response:</span></span>
> <span data-ttu-id="3da26-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3da26-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


