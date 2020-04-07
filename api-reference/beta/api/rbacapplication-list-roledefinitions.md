---
title: Listar unifiedRoleDefinitions
description: Obtenha uma lista de objetos unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d5c161ed6144ebdc7300935702891e6aa244113
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160272"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="89b21-103">Listar unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="89b21-103">List unifiedRoleDefinitions</span></span>

<span data-ttu-id="89b21-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89b21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89b21-105">Obtenha uma lista de objetos [unifiedRoleDefinition](../resources/unifiedroledefinition.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="89b21-105">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="89b21-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="89b21-106">Permissions</span></span>

<span data-ttu-id="89b21-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89b21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89b21-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89b21-109">Permission type</span></span>      | <span data-ttu-id="89b21-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="89b21-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89b21-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89b21-111">Delegated (work or school account)</span></span> | <span data-ttu-id="89b21-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="89b21-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="89b21-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89b21-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89b21-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89b21-114">Not supported.</span></span>    |
|<span data-ttu-id="89b21-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89b21-115">Application</span></span> | <span data-ttu-id="89b21-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="89b21-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="89b21-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89b21-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89b21-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="89b21-118">Optional query parameters</span></span>
<span data-ttu-id="89b21-119">Este método é `$filter` compatível `id`com `displayName`o, `isBuiltIn`, e.</span><span class="sxs-lookup"><span data-stu-id="89b21-119">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="89b21-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="89b21-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="89b21-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89b21-121">Request headers</span></span>

| <span data-ttu-id="89b21-122">Nome</span><span class="sxs-lookup"><span data-stu-id="89b21-122">Name</span></span>      |<span data-ttu-id="89b21-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="89b21-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="89b21-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="89b21-124">Authorization</span></span> | <span data-ttu-id="89b21-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="89b21-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="89b21-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89b21-126">Request body</span></span>

<span data-ttu-id="89b21-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="89b21-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89b21-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b21-128">Response</span></span>

<span data-ttu-id="89b21-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89b21-129">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89b21-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89b21-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="89b21-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89b21-131">Request</span></span>

<span data-ttu-id="89b21-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="89b21-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="89b21-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="89b21-133">Response</span></span>

<span data-ttu-id="89b21-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="89b21-134">The following is an example of the response.</span></span>

> <span data-ttu-id="89b21-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89b21-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->