---
title: Atualizar um oAuth2PermissionGrant
description: Atualize as propriedades de um oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0c9d3f60eeff2edd01d6926fb2fed18a3e508db4
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447886"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="db36f-103">Atualizar uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="db36f-103">Update a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="db36f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db36f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db36f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db36f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db36f-106">Atualize as propriedades do [objeto oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) representando uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="db36f-106">Update the properties of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object, representing a delegated permission grant.</span></span>

<span data-ttu-id="db36f-107">Um **oAuth2PermissionGrant** pode ser atualizado para alterar quais permissões delegadas são **concedidas,** adicionando ou removendo itens da lista em escopos .</span><span class="sxs-lookup"><span data-stu-id="db36f-107">An **oAuth2PermissionGrant** can be updated to change which delegated permissions are granted, by adding or removing items from the list in **scopes**.</span></span>

## <a name="permissions"></a><span data-ttu-id="db36f-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="db36f-108">Permissions</span></span>

<span data-ttu-id="db36f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db36f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db36f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db36f-111">Permission type</span></span>      | <span data-ttu-id="db36f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="db36f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db36f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db36f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="db36f-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="db36f-114">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="db36f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db36f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db36f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db36f-116">Not supported.</span></span>    |
|<span data-ttu-id="db36f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db36f-117">Application</span></span> | <span data-ttu-id="db36f-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db36f-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db36f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db36f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db36f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db36f-120">Request headers</span></span>

| <span data-ttu-id="db36f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="db36f-121">Name</span></span>       | <span data-ttu-id="db36f-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="db36f-122">Type</span></span> | <span data-ttu-id="db36f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="db36f-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="db36f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="db36f-124">Authorization</span></span>  | <span data-ttu-id="db36f-125">string</span><span class="sxs-lookup"><span data-stu-id="db36f-125">string</span></span>  | <span data-ttu-id="db36f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db36f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db36f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db36f-128">Request body</span></span>

<span data-ttu-id="db36f-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="db36f-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="db36f-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db36f-132">Property</span></span>     | <span data-ttu-id="db36f-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="db36f-133">Type</span></span>   |<span data-ttu-id="db36f-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="db36f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db36f-135">scope</span><span class="sxs-lookup"><span data-stu-id="db36f-135">scope</span></span>|<span data-ttu-id="db36f-136">String</span><span class="sxs-lookup"><span data-stu-id="db36f-136">String</span></span>| <span data-ttu-id="db36f-137">Especifica o valor da declaração de escopo que o aplicativo de recurso deve esperar no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="db36f-137">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="db36f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="db36f-138">Response</span></span>

<span data-ttu-id="db36f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db36f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db36f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db36f-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="db36f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db36f-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="db36f-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="db36f-143">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/beta/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```

# <a name="c"></a>[<span data-ttu-id="db36f-144">C#</span><span class="sxs-lookup"><span data-stu-id="db36f-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db36f-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db36f-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db36f-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db36f-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db36f-147">Java</span><span class="sxs-lookup"><span data-stu-id="db36f-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="db36f-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="db36f-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update oAuth2PermissionGrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


