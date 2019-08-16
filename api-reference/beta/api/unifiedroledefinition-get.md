---
title: Obter unifiedRoleDefinition
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5c4eb302ce22678b28490caedacecfac9896dd61
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437759"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="9a0c8-103">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9a0c8-103">Get unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a0c8-104">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9a0c8-104">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="9a0c8-105">Atualmente, "Directory" é o único aplicativo RBAC compatível.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-105">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a0c8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a0c8-106">Permissions</span></span>

<span data-ttu-id="9a0c8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a0c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a0c8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a0c8-109">Permission type</span></span>      | <span data-ttu-id="9a0c8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a0c8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a0c8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a0c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a0c8-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="9a0c8-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a0c8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a0c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a0c8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-114">Not supported.</span></span>    |
|<span data-ttu-id="9a0c8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a0c8-115">Application</span></span> | <span data-ttu-id="9a0c8-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="9a0c8-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a0c8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a0c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/{rbacApplication}/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a0c8-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a0c8-118">Optional query parameters</span></span>

<span data-ttu-id="9a0c8-119">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="9a0c8-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9a0c8-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a0c8-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0c8-121">Request headers</span></span>

| <span data-ttu-id="9a0c8-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9a0c8-122">Name</span></span>      |<span data-ttu-id="9a0c8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a0c8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a0c8-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a0c8-124">Authorization</span></span> | <span data-ttu-id="9a0c8-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="9a0c8-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a0c8-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0c8-126">Request body</span></span>

<span data-ttu-id="9a0c8-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a0c8-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0c8-128">Response</span></span>

<span data-ttu-id="9a0c8-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a0c8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a0c8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a0c8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a0c8-131">Request</span></span>

<span data-ttu-id="9a0c8-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```

### <a name="response"></a><span data-ttu-id="9a0c8-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a0c8-133">Response</span></span>

<span data-ttu-id="9a0c8-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-134">The following is an example of the response.</span></span>

> <span data-ttu-id="9a0c8-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a0c8-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions/$entity",
    "id": "f189965f-f560-4c59-9101-933d4c87a91a",
    "description": "Allows reading Application Registrations",
    "displayName": "Application Registration Reader",
    "isBuiltIn": false,
    "isEnabled": true,
    "resourceScopes": [
        "/"
    ],
    "templateId": "429c3819-053d-4250-9926-4c7dcb18ae17",
    "version": null,
    "rolePermissions": [
        {
            "allowedResourceActions": [
                "microsoft.directory/applications/allProperties/read"
            ],
            "condition": null
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->