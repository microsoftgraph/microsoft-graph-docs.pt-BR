---
title: Excluir unifiedRoleDefinition
description: Excluir um objeto unifiedRoleDefinition.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6e0d097732c58285c50004c4416e602960106acb
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437843"
---
# <a name="delete-unifiedroledefinition"></a><span data-ttu-id="837df-103">Excluir unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="837df-103">Delete unifiedRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="837df-104">Excluir um objeto [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="837df-104">Delete a [unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="837df-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="837df-105">Permissions</span></span>

<span data-ttu-id="837df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="837df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="837df-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="837df-108">Permission type</span></span>                        | <span data-ttu-id="837df-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="837df-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="837df-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="837df-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="837df-111">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="837df-111">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |
| <span data-ttu-id="837df-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="837df-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="837df-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="837df-113">Not supported.</span></span> |
| <span data-ttu-id="837df-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="837df-114">Application</span></span>                            | <span data-ttu-id="837df-115">RoleManagement. Read. Directory, RoleManagement. ReadWrite. Directory</span><span class="sxs-lookup"><span data-stu-id="837df-115">RoleManagement.Read.Directory, RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="837df-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="837df-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /roleManagement/directory/roleDefinitions/{id}

```

## <a name="request-headers"></a><span data-ttu-id="837df-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="837df-117">Request headers</span></span>

| <span data-ttu-id="837df-118">Nome</span><span class="sxs-lookup"><span data-stu-id="837df-118">Name</span></span>          | <span data-ttu-id="837df-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="837df-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="837df-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="837df-120">Authorization</span></span> | <span data-ttu-id="837df-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="837df-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="837df-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="837df-122">Request body</span></span>

<span data-ttu-id="837df-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="837df-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="837df-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="837df-124">Response</span></span>

<span data-ttu-id="837df-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="837df-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="837df-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="837df-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="837df-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="837df-128">Request</span></span>

<span data-ttu-id="837df-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="837df-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_unifiedroledefinition"
}-->

```http
DELETE https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a
```

### <a name="response"></a><span data-ttu-id="837df-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="837df-130">Response</span></span>

<span data-ttu-id="837df-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="837df-131">The following is an example of the response.</span></span>

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
  "description": "Delete unifiedRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->