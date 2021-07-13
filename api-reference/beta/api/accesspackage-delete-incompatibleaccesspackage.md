---
title: Remover accessPackage de incompatívelAccessPackages
description: Remova um link que indica que um pacote de acesso é incompatível com um pacote de acesso especificado.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7cb6ad4af6809c75edef5f5e2966eee72a357215
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401021"
---
# <a name="remove-accesspackage-from-incompatibleaccesspackages"></a><span data-ttu-id="ba11f-103">Remover accessPackage de incompatívelAccessPackages</span><span class="sxs-lookup"><span data-stu-id="ba11f-103">Remove accessPackage from incompatibleAccessPackages</span></span>

<span data-ttu-id="ba11f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba11f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba11f-105">Remover um [pacote de](../resources/accesspackage.md) acesso da lista de pacotes de acesso que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="ba11f-105">Remove an [access package](../resources/accesspackage.md) from the list of access packages that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="ba11f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba11f-106">Permissions</span></span>

<span data-ttu-id="ba11f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba11f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba11f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba11f-109">Permission type</span></span>                        | <span data-ttu-id="ba11f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba11f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba11f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba11f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba11f-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba11f-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="ba11f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba11f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba11f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba11f-114">Not supported.</span></span> |
| <span data-ttu-id="ba11f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba11f-115">Application</span></span>                            | <span data-ttu-id="ba11f-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba11f-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba11f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba11f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ba11f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba11f-118">Request headers</span></span>

| <span data-ttu-id="ba11f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ba11f-119">Name</span></span>          | <span data-ttu-id="ba11f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba11f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ba11f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba11f-121">Authorization</span></span> | <span data-ttu-id="ba11f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba11f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ba11f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba11f-124">Content-Type</span></span>  | <span data-ttu-id="ba11f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba11f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba11f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba11f-127">Request body</span></span>

<span data-ttu-id="ba11f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba11f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba11f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba11f-129">Response</span></span>

<span data-ttu-id="ba11f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ba11f-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ba11f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba11f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba11f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba11f-133">Request</span></span>

<span data-ttu-id="ba11f-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba11f-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_incompatibleaccesspackage_from_accesspackage"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages/{id}/$ref
```


### <a name="response"></a><span data-ttu-id="ba11f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba11f-135">Response</span></span>

<span data-ttu-id="ba11f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba11f-136">The following is an example of the response.</span></span>

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
  "description": "Remove incompatibleAccessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

