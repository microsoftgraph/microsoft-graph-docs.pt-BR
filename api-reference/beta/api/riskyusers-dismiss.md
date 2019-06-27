---
title: Ignorar riskyUser
description: Descartar o risco de um objeto riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: b88070f32a021f1d79aa85c091cadc52f2f600ea
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264985"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="a949c-103">riskyUser: fechar</span><span class="sxs-lookup"><span data-stu-id="a949c-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="a949c-104">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="a949c-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="a949c-105">Descarte o risco de um ou mais objetos [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="a949c-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="a949c-106">Esta ação define o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="a949c-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="a949c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a949c-107">Permissions</span></span>
<span data-ttu-id="a949c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a949c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a949c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a949c-110">Permission type</span></span>      | <span data-ttu-id="a949c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a949c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a949c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a949c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a949c-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a949c-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="a949c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a949c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a949c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a949c-115">Not supported.</span></span>    |
|<span data-ttu-id="a949c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a949c-116">Application</span></span> | <span data-ttu-id="a949c-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a949c-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a949c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a949c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="a949c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a949c-119">Request headers</span></span>
| <span data-ttu-id="a949c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a949c-120">Name</span></span>      |<span data-ttu-id="a949c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a949c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a949c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a949c-122">Authorization</span></span>  | <span data-ttu-id="a949c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a949c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a949c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a949c-125">Request body</span></span>
<span data-ttu-id="a949c-126">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a949c-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="a949c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a949c-127">Response</span></span>

<span data-ttu-id="a949c-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a949c-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a949c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a949c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a949c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a949c-131">Request</span></span>
<span data-ttu-id="a949c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a949c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss
Content-Type: application/json

{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="a949c-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a949c-133">Response</span></span>
<span data-ttu-id="a949c-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a949c-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a949c-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a949c-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a949c-136">C#</span><span class="sxs-lookup"><span data-stu-id="a949c-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a949c-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="a949c-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a949c-138">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a949c-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
