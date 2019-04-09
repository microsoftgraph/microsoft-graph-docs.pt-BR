---
title: Ignorar riskyUsers
description: DesCartar o risco de um objeto riskyUsers.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 3027320b25c35e60e1b5dccabc7ff34ea642a953
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/09/2019
ms.locfileid: "31560098"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="a9392-103">Ignorar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="a9392-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="a9392-104">**Observação:** O uso da API riskyUsers requer uma licença do Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="a9392-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="a9392-105">DesCartar o risco de um objeto **riskyUser** .</span><span class="sxs-lookup"><span data-stu-id="a9392-105">Dismiss the risk of a **riskyUser** object.</span></span> <span data-ttu-id="a9392-106">Esta ação definirá o nível de risco do usuário de destino como nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9392-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9392-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a9392-107">Permissions</span></span>
<span data-ttu-id="a9392-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9392-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9392-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9392-110">Permission type</span></span>      | <span data-ttu-id="a9392-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a9392-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9392-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9392-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a9392-113">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a9392-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9392-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9392-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9392-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9392-115">Not supported.</span></span>    |
|<span data-ttu-id="a9392-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9392-116">Application</span></span> | <span data-ttu-id="a9392-117">Identityriskuser. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a9392-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9392-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9392-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="a9392-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9392-119">Request headers</span></span>
| <span data-ttu-id="a9392-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a9392-120">Name</span></span>      |<span data-ttu-id="a9392-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9392-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9392-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9392-122">Authorization</span></span>  | <span data-ttu-id="a9392-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9392-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a9392-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a9392-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="a9392-126">ID da sessão da pasta de trabalho que determina se as alterações são persistentes.</span><span class="sxs-lookup"><span data-stu-id="a9392-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="a9392-127">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a9392-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9392-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9392-128">Request body</span></span>
<span data-ttu-id="a9392-129">Especifique as userIds a serem descartadas no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9392-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="a9392-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9392-130">Response</span></span>

<span data-ttu-id="a9392-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9392-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9392-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9392-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9392-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9392-134">Request</span></span>
<span data-ttu-id="a9392-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9392-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="a9392-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9392-136">Response</span></span>
<span data-ttu-id="a9392-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9392-137">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
