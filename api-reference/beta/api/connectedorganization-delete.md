---
title: Excluir connectedOrganization
description: Exclua connectedOrganization.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f91652b8f7ec479892c6f19d9804b39b521fe58
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509943"
---
# <a name="delete-connectedorganization"></a><span data-ttu-id="24feb-103">Excluir connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="24feb-103">Delete connectedOrganization</span></span>

<span data-ttu-id="24feb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24feb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24feb-105">Excluir um objeto [connectedOrganization](../resources/connectedorganization.md) .</span><span class="sxs-lookup"><span data-stu-id="24feb-105">Delete a [connectedOrganization](../resources/connectedorganization.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="24feb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24feb-106">Permissions</span></span>

<span data-ttu-id="24feb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24feb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24feb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24feb-109">Permission type</span></span>|<span data-ttu-id="24feb-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="24feb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="24feb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24feb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24feb-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24feb-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="24feb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24feb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24feb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24feb-114">Not supported.</span></span> |
| <span data-ttu-id="24feb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24feb-115">Application</span></span>                            | <span data-ttu-id="24feb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24feb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="24feb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24feb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
DELETE /identityGovernance/entitlementManagement/connectedOrganizations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="24feb-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24feb-118">Request headers</span></span>
|<span data-ttu-id="24feb-119">Nome</span><span class="sxs-lookup"><span data-stu-id="24feb-119">Name</span></span>|<span data-ttu-id="24feb-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="24feb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24feb-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="24feb-121">Authorization</span></span>|<span data-ttu-id="24feb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24feb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24feb-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24feb-124">Request body</span></span>
<span data-ttu-id="24feb-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24feb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24feb-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="24feb-126">Response</span></span>

<span data-ttu-id="24feb-127">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="24feb-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="24feb-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24feb-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24feb-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24feb-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_connectedorganization"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations/{id}
```


### <a name="response"></a><span data-ttu-id="24feb-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="24feb-130">Response</span></span>
<span data-ttu-id="24feb-131">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24feb-131">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete connectedOrganization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
