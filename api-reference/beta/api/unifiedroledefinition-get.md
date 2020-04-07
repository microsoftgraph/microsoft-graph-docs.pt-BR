---
title: Obter unifiedRoleDefinition
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 28b402aea4ea857912f150ada2665e9094b4bc00
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2020
ms.locfileid: "43160314"
---
# <a name="get-unifiedroledefinition"></a><span data-ttu-id="68034-103">Obter unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="68034-103">Get unifiedRoleDefinition</span></span>

<span data-ttu-id="68034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68034-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68034-105">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="68034-105">Retrieve the properties and relationships of a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span> <span data-ttu-id="68034-106">Atualmente, "Directory" é o único aplicativo RBAC compatível.</span><span class="sxs-lookup"><span data-stu-id="68034-106">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="68034-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="68034-107">Permissions</span></span>

<span data-ttu-id="68034-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68034-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68034-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68034-110">Permission type</span></span>      | <span data-ttu-id="68034-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68034-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68034-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68034-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68034-113">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="68034-113">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68034-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68034-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68034-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68034-115">Not supported.</span></span>    |
|<span data-ttu-id="68034-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68034-116">Application</span></span> | <span data-ttu-id="68034-117">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="68034-117">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68034-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68034-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/{rbacApplication}/roleDefinitions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68034-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68034-119">Optional query parameters</span></span>

<span data-ttu-id="68034-120">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68034-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="68034-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="68034-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="68034-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68034-122">Request headers</span></span>

| <span data-ttu-id="68034-123">Nome</span><span class="sxs-lookup"><span data-stu-id="68034-123">Name</span></span>      |<span data-ttu-id="68034-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="68034-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="68034-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="68034-125">Authorization</span></span> | <span data-ttu-id="68034-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="68034-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="68034-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68034-127">Request body</span></span>

<span data-ttu-id="68034-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68034-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68034-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="68034-129">Response</span></span>

<span data-ttu-id="68034-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [unifiedRoleDefinition](../resources/unifiedroledefinition.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68034-130">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68034-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68034-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="68034-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68034-132">Request</span></span>

<span data-ttu-id="68034-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68034-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_unifiedroledefinition"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```

### <a name="response"></a><span data-ttu-id="68034-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="68034-134">Response</span></span>

<span data-ttu-id="68034-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68034-135">The following is an example of the response.</span></span>

> <span data-ttu-id="68034-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68034-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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