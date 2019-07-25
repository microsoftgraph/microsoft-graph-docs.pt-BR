---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: ca2cbaacdc84f7c7aee3f1894beef562dd094ba9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871034"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="847ac-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="847ac-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="847ac-104">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="847ac-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="847ac-105">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="847ac-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="847ac-106">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="847ac-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="847ac-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="847ac-107">Permissions</span></span>
<span data-ttu-id="847ac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="847ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="847ac-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="847ac-110">Permission type</span></span>      | <span data-ttu-id="847ac-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="847ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="847ac-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="847ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="847ac-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="847ac-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="847ac-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="847ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="847ac-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="847ac-115">Not supported.</span></span>    |
|<span data-ttu-id="847ac-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="847ac-116">Application</span></span> | <span data-ttu-id="847ac-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="847ac-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="847ac-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="847ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="847ac-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="847ac-119">Request headers</span></span>
| <span data-ttu-id="847ac-120">Nome</span><span class="sxs-lookup"><span data-stu-id="847ac-120">Name</span></span>      |<span data-ttu-id="847ac-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="847ac-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="847ac-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="847ac-122">Authorization</span></span>  | <span data-ttu-id="847ac-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="847ac-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="847ac-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="847ac-125">Request body</span></span>
<span data-ttu-id="847ac-126">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="847ac-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="847ac-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="847ac-127">Response</span></span>

<span data-ttu-id="847ac-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="847ac-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="847ac-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="847ac-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="847ac-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="847ac-131">Request</span></span>
<span data-ttu-id="847ac-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="847ac-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="847ac-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="847ac-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "confirm_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/confirmCompromised
Content-type: application/json

{
  "userIds": [
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="847ac-134">C#</span><span class="sxs-lookup"><span data-stu-id="847ac-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="847ac-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="847ac-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="847ac-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="847ac-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="847ac-137">Java</span><span class="sxs-lookup"><span data-stu-id="847ac-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/confirm-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="847ac-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="847ac-138">Response</span></span>
<span data-ttu-id="847ac-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="847ac-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
