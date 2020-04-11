---
title: Atribuir tokenIssuancePolicy
description: Atribuir um tokenIssuancePolicy a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9fb13280c5998926933efb5cbf6aa265cb17ab4f
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227763"
---
# <a name="assign-tokenissuancepolicy"></a><span data-ttu-id="8bc13-103">Atribuir tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="8bc13-103">Assign tokenIssuancePolicy</span></span>

<span data-ttu-id="8bc13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bc13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8bc13-105">Atribuir um [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="8bc13-105">Assign a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bc13-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8bc13-106">Permissions</span></span>

<span data-ttu-id="8bc13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8bc13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bc13-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8bc13-109">Permission type</span></span>                        | <span data-ttu-id="8bc13-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8bc13-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8bc13-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8bc13-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bc13-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8bc13-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="8bc13-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8bc13-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bc13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8bc13-114">Not supported.</span></span> |
| <span data-ttu-id="8bc13-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8bc13-115">Application</span></span>                            | <span data-ttu-id="8bc13-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="8bc13-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bc13-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8bc13-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenIssuancePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="8bc13-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc13-118">Request headers</span></span>

| <span data-ttu-id="8bc13-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8bc13-119">Name</span></span>          | <span data-ttu-id="8bc13-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8bc13-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8bc13-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8bc13-121">Authorization</span></span> | <span data-ttu-id="8bc13-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc13-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8bc13-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8bc13-124">Content-Type</span></span> | <span data-ttu-id="8bc13-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8bc13-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bc13-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc13-127">Request body</span></span>

<span data-ttu-id="8bc13-128">No corpo da solicitação, forneça o identificador do objeto [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8bc13-128">In the request body, supply the identifier of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object (using an `@odata.id` property) that should be assigned to the application.</span></span>

## <a name="response"></a><span data-ttu-id="8bc13-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bc13-129">Response</span></span>

<span data-ttu-id="8bc13-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8bc13-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bc13-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8bc13-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bc13-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8bc13-133">Request</span></span>

<span data-ttu-id="8bc13-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8bc13-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="8bc13-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8bc13-135">Response</span></span>

<span data-ttu-id="8bc13-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8bc13-136">The following is an example of the response.</span></span>

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
  "description": "Assign tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
