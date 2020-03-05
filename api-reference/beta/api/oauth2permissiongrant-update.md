---
title: Atualizar oAuth2PermissionGrant
description: Atualize as propriedades do objeto oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 056b1491de7044efac3a51612590766949fd7a96
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456611"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="bbc5d-103">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="bbc5d-103">Update oAuth2PermissionGrant</span></span>

<span data-ttu-id="bbc5d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bbc5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbc5d-105">Atualize as propriedades do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="bbc5d-105">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bbc5d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbc5d-106">Permissions</span></span>

<span data-ttu-id="bbc5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbc5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bbc5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbc5d-109">Permission type</span></span>      | <span data-ttu-id="bbc5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbc5d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbc5d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbc5d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bbc5d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bbc5d-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bbc5d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbc5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbc5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbc5d-114">Not supported.</span></span>    |
|<span data-ttu-id="bbc5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbc5d-115">Application</span></span> | <span data-ttu-id="bbc5d-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbc5d-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbc5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc5d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bbc5d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc5d-118">Request headers</span></span>
| <span data-ttu-id="bbc5d-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bbc5d-119">Name</span></span>       | <span data-ttu-id="bbc5d-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbc5d-120">Type</span></span> | <span data-ttu-id="bbc5d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbc5d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bbc5d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbc5d-122">Authorization</span></span>  | <span data-ttu-id="bbc5d-123">string</span><span class="sxs-lookup"><span data-stu-id="bbc5d-123">string</span></span>  | <span data-ttu-id="bbc5d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbc5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbc5d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc5d-126">Request body</span></span>
<span data-ttu-id="bbc5d-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bbc5d-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bbc5d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbc5d-130">Property</span></span>     | <span data-ttu-id="bbc5d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbc5d-131">Type</span></span>   |<span data-ttu-id="bbc5d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbc5d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbc5d-133">scope</span><span class="sxs-lookup"><span data-stu-id="bbc5d-133">scope</span></span>|<span data-ttu-id="bbc5d-134">String</span><span class="sxs-lookup"><span data-stu-id="bbc5d-134">String</span></span>| <span data-ttu-id="bbc5d-135">Especifica o valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="bbc5d-135">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="bbc5d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbc5d-136">Response</span></span>

<span data-ttu-id="bbc5d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbc5d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbc5d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbc5d-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbc5d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbc5d-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bbc5d-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bbc5d-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_oAuth2Permissiongrant"
}-->
```http
PATCH https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
Content-type: application/json
Content-length: 30

{
  "scope": "scope-value"
}
```
# <a name="c"></a>[<span data-ttu-id="bbc5d-142">C#</span><span class="sxs-lookup"><span data-stu-id="bbc5d-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bbc5d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bbc5d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bbc5d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bbc5d-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bbc5d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbc5d-145">Response</span></span>

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
  "description": "Update oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
