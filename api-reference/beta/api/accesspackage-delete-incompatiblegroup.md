---
title: Remover grupo de incompatibleGroups
description: Remova um link que indica que um grupo é incompatível com um pacote de acesso especificado.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 9dab2d0aa8278f932648106e2db87eef513aeebd
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401019"
---
# <a name="remove-group-from-incompatiblegroups"></a><span data-ttu-id="4a7fc-103">Remover grupo de incompatibleGroups</span><span class="sxs-lookup"><span data-stu-id="4a7fc-103">Remove group from incompatibleGroups</span></span>

<span data-ttu-id="4a7fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a7fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a7fc-105">Remover um [grupo](../resources/group.md) da lista de grupos que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="4a7fc-105">Remove a [group](../resources/group.md) from the list of groups that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="4a7fc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4a7fc-106">Permissions</span></span>

<span data-ttu-id="4a7fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a7fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a7fc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a7fc-109">Permission type</span></span>                        | <span data-ttu-id="4a7fc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a7fc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a7fc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a7fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a7fc-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7fc-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4a7fc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a7fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a7fc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-114">Not supported.</span></span> |
| <span data-ttu-id="4a7fc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a7fc-115">Application</span></span>                            | <span data-ttu-id="4a7fc-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a7fc-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a7fc-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a7fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4a7fc-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a7fc-118">Request headers</span></span>

| <span data-ttu-id="4a7fc-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4a7fc-119">Name</span></span>          | <span data-ttu-id="4a7fc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a7fc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4a7fc-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a7fc-121">Authorization</span></span> | <span data-ttu-id="4a7fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4a7fc-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a7fc-124">Content-Type</span></span>  | <span data-ttu-id="4a7fc-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a7fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a7fc-127">Request body</span></span>

<span data-ttu-id="4a7fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a7fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a7fc-129">Response</span></span>

<span data-ttu-id="4a7fc-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a7fc-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4a7fc-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a7fc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a7fc-133">Request</span></span>

<span data-ttu-id="4a7fc-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_incompatiblegroup_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups/{id}/$ref
```


### <a name="response"></a><span data-ttu-id="4a7fc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a7fc-135">Response</span></span>

<span data-ttu-id="4a7fc-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4a7fc-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove incompatibleGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


