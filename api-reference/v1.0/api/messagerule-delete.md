---
title: Excluir messageRule
description: Exclua o objeto messageRule especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 570970296444b5bb4d5033bf26a03214d9fa8dac
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957358"
---
# <a name="delete-messagerule"></a><span data-ttu-id="b8383-103">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="b8383-103">Delete messageRule</span></span>


<span data-ttu-id="b8383-104">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="b8383-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8383-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8383-105">Permissions</span></span>
<span data-ttu-id="b8383-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8383-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8383-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8383-108">Permission type</span></span>      | <span data-ttu-id="b8383-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8383-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8383-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8383-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8383-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8383-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b8383-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8383-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8383-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8383-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b8383-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8383-114">Application</span></span> | <span data-ttu-id="b8383-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8383-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8383-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8383-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b8383-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8383-117">Request headers</span></span>
| <span data-ttu-id="b8383-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b8383-118">Name</span></span>       | <span data-ttu-id="b8383-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8383-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8383-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8383-120">Authorization</span></span>  | <span data-ttu-id="b8383-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8383-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b8383-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8383-123">Request body</span></span>
<span data-ttu-id="b8383-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8383-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b8383-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8383-125">Response</span></span>
<span data-ttu-id="b8383-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8383-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8383-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8383-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8383-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8383-129">Request</span></span>
<span data-ttu-id="b8383-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b8383-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="b8383-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8383-131">Response</span></span>
<span data-ttu-id="b8383-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8383-132">Here is an example of the response.</span></span> 
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
