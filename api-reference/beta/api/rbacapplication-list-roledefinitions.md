---
title: Listar unifiedRoleDefinitions
description: Obtenha uma lista de objetos unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 642b5582d49930e340d8d879c9b65f7ff4b05e2a
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437696"
---
# <a name="list-unifiedroledefinitions"></a><span data-ttu-id="ab6ff-103">Listar unifiedRoleDefinitions</span><span class="sxs-lookup"><span data-stu-id="ab6ff-103">List unifiedRoleDefinitions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab6ff-104">Obtenha uma lista de objetos [unifiedRoleDefinition](../resources/unifiedroledefinition.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-104">Get a list of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab6ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab6ff-105">Permissions</span></span>

<span data-ttu-id="ab6ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab6ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab6ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab6ff-108">Permission type</span></span>      | <span data-ttu-id="ab6ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab6ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab6ff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab6ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab6ff-111">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ab6ff-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab6ff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab6ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab6ff-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-113">Not supported.</span></span>    |
|<span data-ttu-id="ab6ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab6ff-114">Application</span></span> | <span data-ttu-id="ab6ff-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ab6ff-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab6ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab6ff-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab6ff-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab6ff-117">Optional query parameters</span></span>
<span data-ttu-id="ab6ff-118">Este método é `$filter` compatível `id`com `displayName`o, `isBuiltIn`, e.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-118">This method supports `$filter` on `id`, `displayName`, and `isBuiltIn`.</span></span> <span data-ttu-id="ab6ff-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ab6ff-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab6ff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab6ff-120">Request headers</span></span>

| <span data-ttu-id="ab6ff-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ab6ff-121">Name</span></span>      |<span data-ttu-id="ab6ff-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab6ff-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab6ff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab6ff-123">Authorization</span></span> | <span data-ttu-id="ab6ff-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ab6ff-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab6ff-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab6ff-125">Request body</span></span>

<span data-ttu-id="ab6ff-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab6ff-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab6ff-127">Response</span></span>

<span data-ttu-id="ab6ff-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleDefinition](../resources/unifiedroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-128">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleDefinition](../resources/unifiedroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab6ff-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab6ff-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab6ff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab6ff-130">Request</span></span>

<span data-ttu-id="ab6ff-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="ab6ff-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab6ff-132">Response</span></span>

<span data-ttu-id="ab6ff-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-133">The following is an example of the response.</span></span>

> <span data-ttu-id="ab6ff-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab6ff-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "resourceScopes": [
                "/"
            ],
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
            "resourceScopes": [
                "/"
            ],
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
            "resourceScopes": [
                "/"
            ],
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
