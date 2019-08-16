---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9e73fa6c299589aaf4865a547b600ba59d6e211
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437766"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="5c5ea-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5c5ea-103">Get unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c5ea-104">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5c5ea-104">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5ea-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c5ea-105">Permissions</span></span>

<span data-ttu-id="5c5ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5ea-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c5ea-108">Permission type</span></span>      | <span data-ttu-id="5c5ea-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c5ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c5ea-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c5ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c5ea-111">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="5c5ea-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5c5ea-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c5ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5ea-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-113">Not supported.</span></span>    |
|<span data-ttu-id="5c5ea-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c5ea-114">Application</span></span> | <span data-ttu-id="5c5ea-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="5c5ea-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c5ea-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5ea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c5ea-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c5ea-117">Optional query parameters</span></span>

<span data-ttu-id="5c5ea-118">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-118">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c5ea-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5c5ea-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c5ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5ea-120">Request headers</span></span>

| <span data-ttu-id="5c5ea-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5c5ea-121">Name</span></span>      |<span data-ttu-id="5c5ea-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c5ea-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c5ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c5ea-123">Authorization</span></span> | <span data-ttu-id="5c5ea-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5c5ea-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c5ea-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5ea-125">Request body</span></span>

<span data-ttu-id="5c5ea-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c5ea-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5ea-127">Response</span></span>

<span data-ttu-id="5c5ea-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-128">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c5ea-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5c5ea-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c5ea-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5ea-130">Request</span></span>

<span data-ttu-id="5c5ea-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

### <a name="response"></a><span data-ttu-id="5c5ea-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5ea-132">Response</span></span>

<span data-ttu-id="5c5ea-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-133">The following is an example of the response.</span></span>

> <span data-ttu-id="5c5ea-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5c5ea-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "resourceScope": "/",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->