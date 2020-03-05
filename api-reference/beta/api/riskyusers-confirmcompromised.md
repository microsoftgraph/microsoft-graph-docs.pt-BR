---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
doc_type: apiPageType
ms.openlocfilehash: 1e234ecb92084bc0c180b4b069cfa7f7ce38629a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453881"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="da585-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="da585-103">riskyUser: confirmCompromised</span></span>

<span data-ttu-id="da585-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="da585-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="da585-105">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="da585-105">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="da585-106">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="da585-106">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="da585-107">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="da585-107">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="da585-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="da585-108">Permissions</span></span>
<span data-ttu-id="da585-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da585-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da585-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da585-111">Permission type</span></span>      | <span data-ttu-id="da585-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="da585-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da585-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da585-113">Delegated (work or school account)</span></span> | <span data-ttu-id="da585-114">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da585-114">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="da585-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da585-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da585-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da585-116">Not supported.</span></span>    |
|<span data-ttu-id="da585-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da585-117">Application</span></span> | <span data-ttu-id="da585-118">IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da585-118">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da585-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da585-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="da585-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da585-120">Request headers</span></span>
| <span data-ttu-id="da585-121">Nome</span><span class="sxs-lookup"><span data-stu-id="da585-121">Name</span></span>      |<span data-ttu-id="da585-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="da585-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="da585-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="da585-123">Authorization</span></span>  | <span data-ttu-id="da585-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da585-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="da585-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da585-126">Request body</span></span>
<span data-ttu-id="da585-127">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da585-127">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="da585-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="da585-128">Response</span></span>

<span data-ttu-id="da585-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da585-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da585-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da585-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da585-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da585-132">Request</span></span>
<span data-ttu-id="da585-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da585-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da585-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="da585-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="da585-135">C#</span><span class="sxs-lookup"><span data-stu-id="da585-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/confirm-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da585-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da585-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/confirm-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da585-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da585-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/confirm-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da585-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="da585-138">Response</span></span>
<span data-ttu-id="da585-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da585-139">Here is an example of the response.</span></span>
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
