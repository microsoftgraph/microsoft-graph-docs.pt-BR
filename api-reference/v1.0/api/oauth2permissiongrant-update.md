---
title: Atualizar um oAuth2PermissionGrant
description: Atualize as propriedades de um oAuth2PermissionGrant, representando uma concessão de permissão delegada.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: fd75e020e69888c81cf4a9c53c180585ace73c7e
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441771"
---
# <a name="update-a-delegated-permission-grant-oauth2permissiongrant"></a><span data-ttu-id="ad59e-103">Atualizar uma concessão de permissão delegada (oAuth2PermissionGrant)</span><span class="sxs-lookup"><span data-stu-id="ad59e-103">Update a delegated permission grant (oAuth2PermissionGrant)</span></span>

<span data-ttu-id="ad59e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad59e-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="ad59e-105">Atualize as propriedades do [objeto oAuth2PermissionGrant,](../resources/oauth2permissiongrant.md) representando uma concessão de permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="ad59e-105">Update the properties of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object, representing a delegated permission grant.</span></span>

<span data-ttu-id="ad59e-106">Um **oAuth2PermissionGrant** pode ser atualizado para alterar quais permissões delegadas são **concedidas,** adicionando ou removendo itens da lista em escopos .</span><span class="sxs-lookup"><span data-stu-id="ad59e-106">An **oAuth2PermissionGrant** can be updated to change which delegated permissions are granted, by adding or removing items from the list in **scopes**.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad59e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad59e-107">Permissions</span></span>

<span data-ttu-id="ad59e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad59e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad59e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad59e-110">Permission type</span></span>      | <span data-ttu-id="ad59e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad59e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad59e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad59e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ad59e-113">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad59e-113">DelegatedPermissionGrant.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad59e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad59e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad59e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad59e-115">Not supported.</span></span>    |
|<span data-ttu-id="ad59e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad59e-116">Application</span></span> | <span data-ttu-id="ad59e-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad59e-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad59e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad59e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oauth2PermissionGrants/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ad59e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad59e-119">Request headers</span></span>

| <span data-ttu-id="ad59e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ad59e-120">Name</span></span>       | <span data-ttu-id="ad59e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad59e-121">Type</span></span> | <span data-ttu-id="ad59e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad59e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ad59e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad59e-123">Authorization</span></span>  | <span data-ttu-id="ad59e-124">string</span><span class="sxs-lookup"><span data-stu-id="ad59e-124">string</span></span>  | <span data-ttu-id="ad59e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ad59e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad59e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad59e-127">Request body</span></span>

<span data-ttu-id="ad59e-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ad59e-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ad59e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad59e-131">Property</span></span>     | <span data-ttu-id="ad59e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad59e-132">Type</span></span>   |<span data-ttu-id="ad59e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad59e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad59e-134">scope</span><span class="sxs-lookup"><span data-stu-id="ad59e-134">scope</span></span>|<span data-ttu-id="ad59e-135">String</span><span class="sxs-lookup"><span data-stu-id="ad59e-135">String</span></span>| <span data-ttu-id="ad59e-136">Especifica o valor da declaração de escopo que o aplicativo de recurso deve esperar no token de acesso OAuth 2.0.</span><span class="sxs-lookup"><span data-stu-id="ad59e-136">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="ad59e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad59e-137">Response</span></span>

<span data-ttu-id="ad59e-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad59e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad59e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad59e-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad59e-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad59e-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ad59e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad59e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2PermissionGrant"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/oauth2PermissionGrants/{id}
Content-Type: application/json
Content-Length: 30

{
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="ad59e-143">C#</span><span class="sxs-lookup"><span data-stu-id="ad59e-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad59e-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad59e-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad59e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad59e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad59e-146">Java</span><span class="sxs-lookup"><span data-stu-id="ad59e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-oauth2permissiongrant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad59e-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad59e-147">Response</span></span>

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

