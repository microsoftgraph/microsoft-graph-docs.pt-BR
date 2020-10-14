---
title: Criar permissionGrantPolicy
description: Cria um objeto permissionGrantPolicy que descreve as condições sob as quais as permissões podem ser concedidas.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 4e6c268abee94f81db722249ad31fd97d1c62e48
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458644"
---
# <a name="create-permissiongrantpolicy"></a><span data-ttu-id="061e2-103">Criar permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="061e2-103">Create permissionGrantPolicy</span></span>

<span data-ttu-id="061e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="061e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="061e2-105">Cria um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="061e2-105">Creates a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span> <span data-ttu-id="061e2-106">Uma política de concessão de permissão é usada para descrever as condições sob as quais podem ser concedidas permissões (por exemplo, durante o consentimento do aplicativo).</span><span class="sxs-lookup"><span data-stu-id="061e2-106">A permission grant policy is used to describe the conditions under which permissions can be granted (for example, during application consent).</span></span>

<span data-ttu-id="061e2-107">Após criar a política de concessão de permissão, você pode [Adicionar conjuntos de condições de inclusão](permissiongrantpolicy-post-includes.md) para adicionar regras de correspondência e [Adicionar conjuntos de condições](permissiongrantpolicy-post-excludes.md) de exclusão para adicionar regras de exclusão.</span><span class="sxs-lookup"><span data-stu-id="061e2-107">After creating the permission grant policy, you can [add include condition sets](permissiongrantpolicy-post-includes.md) to add matching rules, and [add exclude condition sets](permissiongrantpolicy-post-excludes.md) to add exclusion rules.</span></span>

## <a name="permissions"></a><span data-ttu-id="061e2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="061e2-108">Permissions</span></span>

<span data-ttu-id="061e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="061e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="061e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="061e2-111">Permission type</span></span>      | <span data-ttu-id="061e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="061e2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="061e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="061e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="061e2-114">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="061e2-114">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="061e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="061e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="061e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="061e2-116">Not supported.</span></span>    |
|<span data-ttu-id="061e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="061e2-117">Application</span></span> | <span data-ttu-id="061e2-118">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="061e2-118">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="061e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="061e2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /policies/permissionGrantPolicies
```

## <a name="request-headers"></a><span data-ttu-id="061e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="061e2-120">Request headers</span></span>

| <span data-ttu-id="061e2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="061e2-121">Name</span></span>       | <span data-ttu-id="061e2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="061e2-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="061e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="061e2-123">Authorization</span></span> | <span data-ttu-id="061e2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="061e2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="061e2-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="061e2-126">Content-type</span></span> | <span data-ttu-id="061e2-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="061e2-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="061e2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="061e2-129">Request body</span></span>

<span data-ttu-id="061e2-130">No corpo da solicitação, forneça uma representação JSON de um objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="061e2-130">In the request body, supply a JSON representation of an [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="061e2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="061e2-131">Response</span></span>

<span data-ttu-id="061e2-132">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [permissionGrantPolicy](../resources/permissiongrantpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="061e2-132">If successful, this method returns a `201 Created` response code and a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="061e2-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="061e2-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="061e2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="061e2-134">Request</span></span>

<span data-ttu-id="061e2-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="061e2-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="061e2-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="061e2-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "truncated": true,
  "name": "create_permissiongrantpolicy"
}-->

```http
POST https://graph.microsoft.com/beta/policies/permissionGrantPolicies
Content-Type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
# <a name="c"></a>[<span data-ttu-id="061e2-137">C#</span><span class="sxs-lookup"><span data-stu-id="061e2-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="061e2-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="061e2-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="061e2-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="061e2-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="061e2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="061e2-140">Response</span></span>

<span data-ttu-id="061e2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="061e2-141">The following is an example of the response.</span></span>

> <span data-ttu-id="061e2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="061e2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "my-custom-consent-policy",
  "displayName": "Custom application consent policy",
  "description": "A custom permission grant policy to customize conditions for granting consent."
}
```
