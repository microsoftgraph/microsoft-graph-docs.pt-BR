---
title: Ignorar riskyUser
description: Descartar o risco de um objeto riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: adf2de791c09075ffcca1b588bd742f48134d409
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447680"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="fa1c8-103">riskyUser: fechar</span><span class="sxs-lookup"><span data-stu-id="fa1c8-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="fa1c8-104">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="fa1c8-105">Descarte o risco de um ou mais objetos [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="fa1c8-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="fa1c8-106">Esta ação define o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="fa1c8-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa1c8-107">Permissions</span></span>
<span data-ttu-id="fa1c8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa1c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa1c8-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa1c8-110">Permission type</span></span>      | <span data-ttu-id="fa1c8-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa1c8-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa1c8-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa1c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa1c8-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa1c8-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa1c8-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa1c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa1c8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-115">Not supported.</span></span>    |
|<span data-ttu-id="fa1c8-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa1c8-116">Application</span></span> | <span data-ttu-id="fa1c8-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa1c8-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa1c8-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa1c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="fa1c8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa1c8-119">Request headers</span></span>
| <span data-ttu-id="fa1c8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fa1c8-120">Name</span></span>      |<span data-ttu-id="fa1c8-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa1c8-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fa1c8-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa1c8-122">Authorization</span></span>  | <span data-ttu-id="fa1c8-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa1c8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa1c8-125">Request body</span></span>
<span data-ttu-id="fa1c8-126">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="fa1c8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa1c8-127">Response</span></span>

<span data-ttu-id="fa1c8-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa1c8-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fa1c8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa1c8-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa1c8-131">Request</span></span>
<span data-ttu-id="fa1c8-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa1c8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa1c8-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa1c8-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa1c8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/dismiss-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa1c8-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa1c8-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/dismiss-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa1c8-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="fa1c8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/dismiss-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fa1c8-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa1c8-137">Response</span></span>
<span data-ttu-id="fa1c8-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa1c8-138">Here is an example of the response.</span></span>
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
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
