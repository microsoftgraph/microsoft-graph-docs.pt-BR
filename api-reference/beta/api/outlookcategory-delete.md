---
title: Excluir categoria do Outlook
description: Exclua o objeto outlookCategory especificado.
author: angelgolfer-ms
ms.openlocfilehash: 114dee21aea5143bd3ad1d6503490ed7941fe6f3
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748231"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="f50a4-103">Excluir categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="f50a4-103">Delete Outlook category</span></span>

> <span data-ttu-id="f50a4-104">**Importante**: APIs sob a versão /beta no Microsoft Graph estiver em Visualizar e estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f50a4-104">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f50a4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f50a4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f50a4-106">Exclua o objeto [outlookCategory](../resources/outlookcategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="f50a4-106">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f50a4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f50a4-107">Permissions</span></span>
<span data-ttu-id="f50a4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f50a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f50a4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f50a4-110">Permission type</span></span>      | <span data-ttu-id="f50a4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f50a4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f50a4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f50a4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f50a4-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f50a4-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f50a4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f50a4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f50a4-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f50a4-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f50a4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f50a4-116">Application</span></span> | <span data-ttu-id="f50a4-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f50a4-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f50a4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f50a4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f50a4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f50a4-119">Request headers</span></span>
| <span data-ttu-id="f50a4-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f50a4-120">Name</span></span>      |<span data-ttu-id="f50a4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f50a4-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f50a4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f50a4-122">Authorization</span></span>  | <span data-ttu-id="f50a4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f50a4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f50a4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f50a4-125">Request body</span></span>
<span data-ttu-id="f50a4-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f50a4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f50a4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f50a4-127">Response</span></span>

<span data-ttu-id="f50a4-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f50a4-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f50a4-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f50a4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f50a4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f50a4-131">Request</span></span>
<span data-ttu-id="f50a4-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f50a4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/masterCategories('4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
```
##### <a name="response"></a><span data-ttu-id="f50a4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f50a4-133">Response</span></span>
<span data-ttu-id="f50a4-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f50a4-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->