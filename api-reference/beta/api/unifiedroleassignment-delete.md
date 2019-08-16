---
title: Excluir unifiedRoleAssignment
description: Excluir um objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9540a1104e2729c65c716a4f64010119b3941ed5
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437780"
---
# <a name="delete-unifiedroleassignment"></a><span data-ttu-id="19904-103">Excluir unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="19904-103">Delete unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19904-104">Excluir um objeto [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) .</span><span class="sxs-lookup"><span data-stu-id="19904-104">Delete a [unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="19904-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="19904-105">Permissions</span></span>

<span data-ttu-id="19904-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19904-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19904-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19904-108">Permission type</span></span>                        | <span data-ttu-id="19904-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19904-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="19904-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19904-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="19904-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="19904-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="19904-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19904-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19904-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19904-113">Not supported.</span></span> |
| <span data-ttu-id="19904-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19904-114">Application</span></span>                            | <span data-ttu-id="19904-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="19904-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="19904-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19904-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleAssignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="19904-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19904-117">Request headers</span></span>

| <span data-ttu-id="19904-118">Nome</span><span class="sxs-lookup"><span data-stu-id="19904-118">Name</span></span>          | <span data-ttu-id="19904-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="19904-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="19904-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="19904-120">Authorization</span></span> | <span data-ttu-id="19904-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="19904-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="19904-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19904-122">Request body</span></span>

<span data-ttu-id="19904-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="19904-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19904-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="19904-124">Response</span></span>

<span data-ttu-id="19904-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19904-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19904-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19904-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="19904-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19904-128">Request</span></span>

<span data-ttu-id="19904-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="19904-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroleassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```

### <a name="response"></a><span data-ttu-id="19904-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="19904-130">Response</span></span>

<span data-ttu-id="19904-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="19904-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
