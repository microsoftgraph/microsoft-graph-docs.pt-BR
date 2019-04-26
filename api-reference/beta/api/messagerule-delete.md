---
title: Excluir messageRule
description: Exclua o objeto messageRule especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 50548749e68fb68b2b33adac2472661da4be9115
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33338323"
---
# <a name="delete-messagerule"></a><span data-ttu-id="6d77e-103">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="6d77e-103">Delete messageRule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d77e-104">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="6d77e-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d77e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d77e-105">Permissions</span></span>
<span data-ttu-id="6d77e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d77e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d77e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d77e-108">Permission type</span></span>      | <span data-ttu-id="6d77e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d77e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d77e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d77e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d77e-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d77e-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6d77e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d77e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d77e-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d77e-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6d77e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d77e-114">Application</span></span> | <span data-ttu-id="6d77e-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6d77e-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d77e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d77e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6d77e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d77e-117">Request headers</span></span>
| <span data-ttu-id="6d77e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6d77e-118">Name</span></span>       | <span data-ttu-id="6d77e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d77e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d77e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d77e-120">Authorization</span></span>  | <span data-ttu-id="6d77e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d77e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6d77e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d77e-123">Request body</span></span>
<span data-ttu-id="6d77e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d77e-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6d77e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d77e-125">Response</span></span>
<span data-ttu-id="6d77e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d77e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d77e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d77e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d77e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d77e-129">Request</span></span>
<span data-ttu-id="6d77e-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d77e-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="6d77e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d77e-131">Response</span></span>
<span data-ttu-id="6d77e-132">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d77e-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
