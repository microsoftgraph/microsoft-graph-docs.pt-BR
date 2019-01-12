---
title: Excluir eventMessage
description: Exclua a eventMessage.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 23007501878f5c5d25af924f3a7e8e1bb618b364
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945955"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="59d6f-103">Excluir eventMessage</span><span class="sxs-lookup"><span data-stu-id="59d6f-103">Delete eventMessage</span></span>

> <span data-ttu-id="59d6f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="59d6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="59d6f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="59d6f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="59d6f-106">Exclua a eventMessage.</span><span class="sxs-lookup"><span data-stu-id="59d6f-106">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="59d6f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="59d6f-107">Permissions</span></span>
<span data-ttu-id="59d6f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59d6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59d6f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59d6f-110">Permission type</span></span>      | <span data-ttu-id="59d6f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59d6f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59d6f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59d6f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59d6f-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d6f-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="59d6f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59d6f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59d6f-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d6f-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="59d6f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59d6f-116">Application</span></span> | <span data-ttu-id="59d6f-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59d6f-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59d6f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59d6f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59d6f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59d6f-119">Request headers</span></span>
| <span data-ttu-id="59d6f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="59d6f-120">Name</span></span>       | <span data-ttu-id="59d6f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="59d6f-121">Type</span></span> | <span data-ttu-id="59d6f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="59d6f-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="59d6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="59d6f-123">Authorization</span></span>  | <span data-ttu-id="59d6f-124">string</span><span class="sxs-lookup"><span data-stu-id="59d6f-124">string</span></span>  | <span data-ttu-id="59d6f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59d6f-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59d6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59d6f-127">Request body</span></span>
<span data-ttu-id="59d6f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59d6f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59d6f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d6f-129">Response</span></span>

<span data-ttu-id="59d6f-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d6f-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59d6f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59d6f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59d6f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59d6f-133">Request</span></span>
<span data-ttu-id="59d6f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="59d6f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="59d6f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="59d6f-135">Response</span></span>
<span data-ttu-id="59d6f-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59d6f-136">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
