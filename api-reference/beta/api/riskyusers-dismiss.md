---
title: Ignorar riskyUser
description: Descartar o risco de um objeto riskyUser.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 2ca876b494b7753918e67ccdff3a6a37a776d054
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639044"
---
# <a name="riskyuser-dismiss"></a><span data-ttu-id="3d740-103">riskyUser: fechar</span><span class="sxs-lookup"><span data-stu-id="3d740-103">riskyUser: dismiss</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="3d740-104">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="3d740-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="3d740-105">Descarte o risco de um ou mais objetos [riskyUser](../resources/riskyuser.md) .</span><span class="sxs-lookup"><span data-stu-id="3d740-105">Dismiss the risk of one or more [riskyUser](../resources/riskyuser.md) objects.</span></span> <span data-ttu-id="3d740-106">Esta ação define o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="3d740-106">This action sets the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="3d740-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="3d740-107">Permissions</span></span>
<span data-ttu-id="3d740-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d740-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d740-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3d740-110">Permission type</span></span>      | <span data-ttu-id="3d740-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3d740-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d740-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3d740-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3d740-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3d740-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d740-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3d740-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d740-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3d740-115">Not supported.</span></span>    |
|<span data-ttu-id="3d740-116">Application</span><span class="sxs-lookup"><span data-stu-id="3d740-116">Application</span></span> | <span data-ttu-id="3d740-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3d740-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d740-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3d740-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="3d740-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3d740-119">Request headers</span></span>
| <span data-ttu-id="3d740-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3d740-120">Name</span></span>      |<span data-ttu-id="3d740-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d740-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d740-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3d740-122">Authorization</span></span>  | <span data-ttu-id="3d740-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3d740-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d740-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3d740-125">Request body</span></span>
<span data-ttu-id="3d740-126">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d740-126">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="3d740-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d740-127">Response</span></span>

<span data-ttu-id="3d740-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d740-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3d740-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3d740-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d740-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3d740-131">Request</span></span>
<span data-ttu-id="3d740-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3d740-132">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="3d740-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3d740-133">Response</span></span>
<span data-ttu-id="3d740-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3d740-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d740-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="3d740-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d740-136">Basic</span><span class="sxs-lookup"><span data-stu-id="3d740-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d740-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d740-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/dismiss_riskyuser-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/riskyusers-dismiss.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
