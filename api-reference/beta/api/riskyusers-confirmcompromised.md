---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: b9c7a4d93a6d7ed493dc7ef231297f1676cbedeb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267071"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="07edb-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="07edb-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="07edb-104">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="07edb-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="07edb-105">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="07edb-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="07edb-106">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="07edb-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="07edb-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="07edb-107">Permissions</span></span>
<span data-ttu-id="07edb-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07edb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07edb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07edb-110">Permission type</span></span>      | <span data-ttu-id="07edb-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07edb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07edb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07edb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="07edb-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="07edb-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="07edb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07edb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07edb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07edb-115">Not supported.</span></span>    |
|<span data-ttu-id="07edb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="07edb-116">Application</span></span> | <span data-ttu-id="07edb-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="07edb-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07edb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07edb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="07edb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07edb-119">Request headers</span></span>
| <span data-ttu-id="07edb-120">Nome</span><span class="sxs-lookup"><span data-stu-id="07edb-120">Name</span></span>      |<span data-ttu-id="07edb-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="07edb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07edb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="07edb-122">Authorization</span></span>  | <span data-ttu-id="07edb-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07edb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07edb-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07edb-125">Request body</span></span>
<span data-ttu-id="07edb-126">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07edb-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="07edb-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="07edb-127">Response</span></span>

<span data-ttu-id="07edb-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07edb-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07edb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07edb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07edb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07edb-131">Request</span></span>
<span data-ttu-id="07edb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07edb-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="07edb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="07edb-133">Response</span></span>
<span data-ttu-id="07edb-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07edb-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="07edb-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="07edb-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07edb-136">C#</span><span class="sxs-lookup"><span data-stu-id="07edb-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07edb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="07edb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="07edb-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="07edb-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Confirm compromised riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
