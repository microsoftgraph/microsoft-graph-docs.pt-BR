---
title: Excluir messageRule
description: Exclua o objeto messageRule especificado.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 85f48f1f293b898cf911488961dade4a1e9962cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807291"
---
# <a name="delete-messagerule"></a><span data-ttu-id="c49f6-103">Excluir messageRule</span><span class="sxs-lookup"><span data-stu-id="c49f6-103">Delete messageRule</span></span>

> <span data-ttu-id="c49f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c49f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c49f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c49f6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c49f6-106">Exclua o objeto [messageRule](../resources/messagerule.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="c49f6-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c49f6-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c49f6-107">Permissions</span></span>
<span data-ttu-id="c49f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c49f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c49f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c49f6-110">Permission type</span></span>      | <span data-ttu-id="c49f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c49f6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c49f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c49f6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c49f6-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c49f6-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c49f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c49f6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c49f6-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c49f6-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c49f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c49f6-116">Application</span></span> | <span data-ttu-id="c49f6-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c49f6-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c49f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c49f6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c49f6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c49f6-119">Request headers</span></span>
| <span data-ttu-id="c49f6-120">Nome</span><span class="sxs-lookup"><span data-stu-id="c49f6-120">Name</span></span>       | <span data-ttu-id="c49f6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c49f6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c49f6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c49f6-122">Authorization</span></span>  | <span data-ttu-id="c49f6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c49f6-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c49f6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c49f6-125">Request body</span></span>
<span data-ttu-id="c49f6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c49f6-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c49f6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c49f6-127">Response</span></span>
<span data-ttu-id="c49f6-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c49f6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c49f6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c49f6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c49f6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c49f6-131">Request</span></span>
<span data-ttu-id="c49f6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c49f6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="c49f6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c49f6-133">Response</span></span>
<span data-ttu-id="c49f6-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c49f6-134">Here is an example of the response.</span></span> 
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
