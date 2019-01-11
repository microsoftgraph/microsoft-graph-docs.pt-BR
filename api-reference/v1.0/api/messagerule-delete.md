---
title: Excluir messageRule
description: Exclua o objeto messageRule especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 2c303ffda5f9f43273178a6b23c72ee465b569dc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842305"
---
# <a name="delete-messagerule"></a><span data-ttu-id="1b2ff-103">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="1b2ff-103">Delete messageRule</span></span>


<span data-ttu-id="1b2ff-104">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="1b2ff-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b2ff-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b2ff-105">Permissions</span></span>
<span data-ttu-id="1b2ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b2ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b2ff-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b2ff-108">Permission type</span></span>      | <span data-ttu-id="1b2ff-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b2ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b2ff-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b2ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1b2ff-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b2ff-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1b2ff-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b2ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b2ff-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b2ff-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1b2ff-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b2ff-114">Application</span></span> | <span data-ttu-id="1b2ff-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1b2ff-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b2ff-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b2ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1b2ff-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2ff-117">Request headers</span></span>
| <span data-ttu-id="1b2ff-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1b2ff-118">Name</span></span>       | <span data-ttu-id="1b2ff-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b2ff-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1b2ff-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b2ff-120">Authorization</span></span>  | <span data-ttu-id="1b2ff-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b2ff-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1b2ff-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2ff-123">Request body</span></span>
<span data-ttu-id="1b2ff-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b2ff-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1b2ff-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b2ff-125">Response</span></span>
<span data-ttu-id="1b2ff-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b2ff-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b2ff-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b2ff-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b2ff-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b2ff-129">Request</span></span>
<span data-ttu-id="1b2ff-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b2ff-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="1b2ff-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b2ff-131">Response</span></span>
<span data-ttu-id="1b2ff-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b2ff-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
