---
title: Atribiur tokenLifetimePolicy
description: Atribuir um tokenLifetimePolicy a um aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9d6b917ac9e819371ab5d91f379c7d69621665b
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229080"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="87643-103">Atribiur tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="87643-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="87643-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87643-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="87643-105">Atribuir um [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) a um [aplicativo](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="87643-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87643-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87643-106">Permissions</span></span>

<span data-ttu-id="87643-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87643-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87643-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87643-109">Permission type</span></span>                        | <span data-ttu-id="87643-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87643-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87643-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87643-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87643-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="87643-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="87643-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87643-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87643-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87643-114">Not supported.</span></span> |
| <span data-ttu-id="87643-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87643-115">Application</span></span>                            | <span data-ttu-id="87643-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="87643-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87643-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87643-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="87643-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87643-118">Request headers</span></span>

| <span data-ttu-id="87643-119">Nome</span><span class="sxs-lookup"><span data-stu-id="87643-119">Name</span></span>          | <span data-ttu-id="87643-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="87643-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="87643-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="87643-121">Authorization</span></span> | <span data-ttu-id="87643-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87643-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87643-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87643-124">Content-Type</span></span> | <span data-ttu-id="87643-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87643-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87643-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87643-127">Request body</span></span>

<span data-ttu-id="87643-128">No corpo da solicitação, forneça o identificador do objeto [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) (usando uma `@odata.id` Propriedade) que deve ser atribuído ao aplicativo ou à entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="87643-128">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="87643-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="87643-129">Response</span></span>

<span data-ttu-id="87643-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87643-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87643-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87643-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="87643-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87643-133">Request</span></span>

<span data-ttu-id="87643-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87643-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/tokenLifetimePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```

### <a name="response"></a><span data-ttu-id="87643-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="87643-135">Response</span></span>

<span data-ttu-id="87643-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87643-136">The following is an example of the response.</span></span>

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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
