---
title: Atualizar oAuth2PermissionGrant
description: Atualize as propriedades do objeto oAuth2PermissionGrant.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 450f7909c6737a623cc23b8622a2817d17ef166d
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2020
ms.locfileid: "43199607"
---
# <a name="update-oauth2permissiongrant"></a><span data-ttu-id="ff0ca-103">Atualizar oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ff0ca-103">Update oAuth2PermissionGrant</span></span>

<span data-ttu-id="ff0ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff0ca-105">Atualize as propriedades do objeto oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="ff0ca-105">Update the properties of oAuth2PermissionGrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff0ca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff0ca-106">Permissions</span></span>

<span data-ttu-id="ff0ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff0ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ff0ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff0ca-109">Permission type</span></span>      | <span data-ttu-id="ff0ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ff0ca-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff0ca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff0ca-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ff0ca-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff0ca-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff0ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff0ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff0ca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff0ca-114">Not supported.</span></span>    |
|<span data-ttu-id="ff0ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff0ca-115">Application</span></span> | <span data-ttu-id="ff0ca-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0ca-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff0ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff0ca-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /oAuth2Permissiongrants/{id}
PATCH /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
PATCH /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ff0ca-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff0ca-118">Request headers</span></span>
| <span data-ttu-id="ff0ca-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ff0ca-119">Name</span></span>       | <span data-ttu-id="ff0ca-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff0ca-120">Type</span></span> | <span data-ttu-id="ff0ca-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff0ca-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff0ca-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff0ca-122">Authorization</span></span>  | <span data-ttu-id="ff0ca-123">string</span><span class="sxs-lookup"><span data-stu-id="ff0ca-123">string</span></span>  | <span data-ttu-id="ff0ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff0ca-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff0ca-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff0ca-126">Request body</span></span>
<span data-ttu-id="ff0ca-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="ff0ca-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ff0ca-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff0ca-130">Property</span></span>     | <span data-ttu-id="ff0ca-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff0ca-131">Type</span></span>   |<span data-ttu-id="ff0ca-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff0ca-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff0ca-133">scope</span><span class="sxs-lookup"><span data-stu-id="ff0ca-133">scope</span></span>|<span data-ttu-id="ff0ca-134">String</span><span class="sxs-lookup"><span data-stu-id="ff0ca-134">String</span></span>| <span data-ttu-id="ff0ca-135">Especifica o valor da declaração do escopo que o aplicativo de recursos deve esperar no token de acesso do OAuth 2,0.</span><span class="sxs-lookup"><span data-stu-id="ff0ca-135">Specifies the value of the scope claim that the resource application should expect in the OAuth 2.0 access token.</span></span> |

## <a name="response"></a><span data-ttu-id="ff0ca-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff0ca-136">Response</span></span>

<span data-ttu-id="ff0ca-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff0ca-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff0ca-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff0ca-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff0ca-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff0ca-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ff0ca-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff0ca-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ff0ca-142">C#</span><span class="sxs-lookup"><span data-stu-id="ff0ca-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ff0ca-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff0ca-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff0ca-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff0ca-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ff0ca-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff0ca-145">Response</span></span>

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
