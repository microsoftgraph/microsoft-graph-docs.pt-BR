---
title: Excluir messageRule
description: Exclua o objeto messageRule especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 570970296444b5bb4d5033bf26a03214d9fa8dac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585209"
---
# <a name="delete-messagerule"></a><span data-ttu-id="58abd-103">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="58abd-103">Delete messageRule</span></span>


<span data-ttu-id="58abd-104">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="58abd-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58abd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="58abd-105">Permissions</span></span>
<span data-ttu-id="58abd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58abd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58abd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58abd-108">Permission type</span></span>      | <span data-ttu-id="58abd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58abd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58abd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58abd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="58abd-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58abd-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="58abd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58abd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58abd-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58abd-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="58abd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58abd-114">Application</span></span> | <span data-ttu-id="58abd-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="58abd-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="58abd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58abd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="58abd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58abd-117">Request headers</span></span>
| <span data-ttu-id="58abd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="58abd-118">Name</span></span>       | <span data-ttu-id="58abd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="58abd-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="58abd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="58abd-120">Authorization</span></span>  | <span data-ttu-id="58abd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58abd-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="58abd-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58abd-123">Request body</span></span>
<span data-ttu-id="58abd-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58abd-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="58abd-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="58abd-125">Response</span></span>
<span data-ttu-id="58abd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58abd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58abd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58abd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="58abd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58abd-129">Request</span></span>
<span data-ttu-id="58abd-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58abd-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="58abd-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="58abd-131">Response</span></span>
<span data-ttu-id="58abd-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58abd-132">Here is an example of the response.</span></span> 
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
