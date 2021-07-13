---
title: Adicionar accessPackage a incompatibleAccessPackages
description: Adicione um link para indicar que um pacote de acesso é incompatível com um pacote de acesso especificado.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1cff2d5fc223253af1827fa503b5bd5d719908eb
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401018"
---
# <a name="add-accesspackage-to-incompatibleaccesspackages"></a><span data-ttu-id="34781-103">Adicionar accessPackage a incompatibleAccessPackages</span><span class="sxs-lookup"><span data-stu-id="34781-103">Add accessPackage to incompatibleAccessPackages</span></span>

<span data-ttu-id="34781-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34781-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34781-105">Adicione um [accessPackage](../resources/accesspackage.md) à lista de pacotes de acesso que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="34781-105">Add an [accessPackage](../resources/accesspackage.md) to the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="34781-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34781-106">Permissions</span></span>

<span data-ttu-id="34781-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="34781-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34781-109">Permission type</span></span>                        | <span data-ttu-id="34781-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34781-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="34781-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34781-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="34781-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34781-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="34781-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34781-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34781-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34781-114">Not supported.</span></span> |
| <span data-ttu-id="34781-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34781-115">Application</span></span>                            | <span data-ttu-id="34781-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34781-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34781-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34781-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref
```

## <a name="request-headers"></a><span data-ttu-id="34781-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34781-118">Request headers</span></span>

| <span data-ttu-id="34781-119">Nome</span><span class="sxs-lookup"><span data-stu-id="34781-119">Name</span></span>          | <span data-ttu-id="34781-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="34781-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="34781-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="34781-121">Authorization</span></span> | <span data-ttu-id="34781-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34781-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="34781-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34781-124">Content-Type</span></span>  | <span data-ttu-id="34781-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34781-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34781-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34781-127">Request body</span></span>

<span data-ttu-id="34781-128">No corpo da solicitação, fornece uma representação JSON de uma estrutura com a id OData do URI de um [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="34781-128">In the request body, supply a JSON representation of a structure with the OData id of the URI of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="34781-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34781-129">Response</span></span>

<span data-ttu-id="34781-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34781-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34781-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="34781-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="34781-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34781-133">Request</span></span>

<span data-ttu-id="34781-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="34781-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "add_incompatibleaccesspackage_to_accesspackage"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/$ref
Content-type: application/json

{
    "@odata.id": "https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2"
}
```

### <a name="response"></a><span data-ttu-id="34781-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="34781-135">Response</span></span>

<span data-ttu-id="34781-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="34781-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Created
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

