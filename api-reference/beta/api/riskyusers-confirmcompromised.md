---
title: Confirmar riskyUser comprometido
description: Confirme um objeto riskyUser como comprometido.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: f0ce7b0a29b90f12104a697bdc38f3297e52676e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639030"
---
# <a name="riskyuser-confirmcompromised"></a><span data-ttu-id="47a36-103">riskyUser: confirmCompromised</span><span class="sxs-lookup"><span data-stu-id="47a36-103">riskyUser: confirmCompromised</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="47a36-104">**Observação:** A API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="47a36-104">**Note:** The riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="47a36-105">Confirme um ou mais objetos [riskyUser](../resources/riskyuser.md) como comprometidos.</span><span class="sxs-lookup"><span data-stu-id="47a36-105">Confirm one or more [riskyUser](../resources/riskyuser.md) objects as compromised.</span></span> <span data-ttu-id="47a36-106">Esta ação define o nível de risco do usuário de destino como alto.</span><span class="sxs-lookup"><span data-stu-id="47a36-106">This action sets the targeted user's risk level to high.</span></span>

## <a name="permissions"></a><span data-ttu-id="47a36-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="47a36-107">Permissions</span></span>
<span data-ttu-id="47a36-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47a36-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a36-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47a36-110">Permission type</span></span>      | <span data-ttu-id="47a36-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47a36-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a36-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47a36-112">Delegated (work or school account)</span></span> | <span data-ttu-id="47a36-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="47a36-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="47a36-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47a36-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47a36-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47a36-115">Not supported.</span></span>    |
|<span data-ttu-id="47a36-116">Application</span><span class="sxs-lookup"><span data-stu-id="47a36-116">Application</span></span> | <span data-ttu-id="47a36-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="47a36-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47a36-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47a36-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/confirmCompromised
```


## <a name="request-headers"></a><span data-ttu-id="47a36-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47a36-119">Request headers</span></span>
| <span data-ttu-id="47a36-120">Nome</span><span class="sxs-lookup"><span data-stu-id="47a36-120">Name</span></span>      |<span data-ttu-id="47a36-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="47a36-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47a36-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="47a36-122">Authorization</span></span>  | <span data-ttu-id="47a36-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47a36-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47a36-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47a36-125">Request body</span></span>
<span data-ttu-id="47a36-126">Especifique as IDs de usuário arriscadas a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47a36-126">Specify the risky user IDs to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="47a36-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a36-127">Response</span></span>

<span data-ttu-id="47a36-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a36-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47a36-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47a36-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47a36-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47a36-131">Request</span></span>
<span data-ttu-id="47a36-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47a36-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="47a36-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a36-133">Response</span></span>
<span data-ttu-id="47a36-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a36-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="47a36-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="47a36-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="47a36-136">Basic</span><span class="sxs-lookup"><span data-stu-id="47a36-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47a36-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47a36-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/confirm_riskyuser-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-confirmcompromised.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
