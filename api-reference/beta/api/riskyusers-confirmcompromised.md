---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 62cad8b9cdad952c5233a6f9ffedd3a16ad6b832
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410861"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="c53a6-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="c53a6-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="c53a6-104">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="c53a6-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="c53a6-105">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="c53a6-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="c53a6-106">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="c53a6-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="c53a6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c53a6-107">Permissions</span></span>
<span data-ttu-id="c53a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c53a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c53a6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c53a6-110">Permission type</span></span>      | <span data-ttu-id="c53a6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c53a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c53a6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c53a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c53a6-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c53a6-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="c53a6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c53a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c53a6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c53a6-115">Not supported.</span></span>    |
|<span data-ttu-id="c53a6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c53a6-116">Application</span></span> | <span data-ttu-id="c53a6-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c53a6-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c53a6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c53a6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="c53a6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c53a6-119">Request headers</span></span>
| <span data-ttu-id="c53a6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c53a6-120">Name</span></span>      |<span data-ttu-id="c53a6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c53a6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c53a6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c53a6-122">Authorization</span></span>  | <span data-ttu-id="c53a6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c53a6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c53a6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c53a6-125">Request body</span></span>
<span data-ttu-id="c53a6-126">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c53a6-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="c53a6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c53a6-127">Response</span></span>

<span data-ttu-id="c53a6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c53a6-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c53a6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c53a6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c53a6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c53a6-131">Request</span></span>
<span data-ttu-id="c53a6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c53a6-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c53a6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c53a6-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="c53a6-134">C#</span><span class="sxs-lookup"><span data-stu-id="c53a6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c53a6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c53a6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c53a6-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c53a6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c53a6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c53a6-137">Response</span></span>
<span data-ttu-id="c53a6-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c53a6-138">Here is an example of the response.</span></span>
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
