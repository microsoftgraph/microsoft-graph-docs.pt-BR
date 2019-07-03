---
title: Atualizar oAuth2PermissionGrant
description: Atualize as propriedades do objeto oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: f29ffb1a9c283014aa26810772f2866dba7ba78d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450055"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="9c4d1-103">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="9c4d1-103">Update oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c4d1-104">Atualize as propriedades do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-104">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c4d1-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9c4d1-105">Permissions</span></span>

<span data-ttu-id="9c4d1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c4d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9c4d1-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c4d1-108">Permission type</span></span>      | <span data-ttu-id="9c4d1-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9c4d1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c4d1-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c4d1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c4d1-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9c4d1-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9c4d1-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c4d1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c4d1-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-113">Not supported.</span></span>    |
|<span data-ttu-id="9c4d1-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c4d1-114">Application</span></span> | <span data-ttu-id="9c4d1-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c4d1-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c4d1-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c4d1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9c4d1-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c4d1-117">Request headers</span></span>
| <span data-ttu-id="9c4d1-118">Nome</span><span class="sxs-lookup"><span data-stu-id="9c4d1-118">Name</span></span>       | <span data-ttu-id="9c4d1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c4d1-119">Type</span></span> | <span data-ttu-id="9c4d1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c4d1-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9c4d1-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c4d1-121">Authorization</span></span>  | <span data-ttu-id="9c4d1-122">string</span><span class="sxs-lookup"><span data-stu-id="9c4d1-122">string</span></span>  | <span data-ttu-id="9c4d1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c4d1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c4d1-125">Request body</span></span>
<span data-ttu-id="9c4d1-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9c4d1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c4d1-129">Property</span></span>     | <span data-ttu-id="9c4d1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c4d1-130">Type</span></span>   |<span data-ttu-id="9c4d1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c4d1-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c4d1-132">scope</span><span class="sxs-lookup"><span data-stu-id="9c4d1-132">scope</span></span>|<span data-ttu-id="9c4d1-133">String</span><span class="sxs-lookup"><span data-stu-id="9c4d1-133">String</span></span>| <span data-ttu-id="9c4d1-134">Especifica o valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-134">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="9c4d1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c4d1-135">Response</span></span>

<span data-ttu-id="9c4d1-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c4d1-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c4d1-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c4d1-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c4d1-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c4d1-139">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="9c4d1-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c4d1-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9c4d1-141">C#</span><span class="sxs-lookup"><span data-stu-id="9c4d1-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9c4d1-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="9c4d1-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9c4d1-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="9c4d1-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c4d1-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c4d1-144">Response</span></span>

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
