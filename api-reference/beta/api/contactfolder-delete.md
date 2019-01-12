---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e8004d726bc8a47270d040ab295bc41dbf1dbef4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980570"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="427e5-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="427e5-103">Delete contactFolder</span></span>

> <span data-ttu-id="427e5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="427e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="427e5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="427e5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="427e5-106">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="427e5-106">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="427e5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="427e5-107">Permissions</span></span>
<span data-ttu-id="427e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="427e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="427e5-110">Permission type</span></span>      | <span data-ttu-id="427e5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="427e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="427e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="427e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="427e5-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="427e5-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="427e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="427e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="427e5-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="427e5-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="427e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="427e5-116">Application</span></span> | <span data-ttu-id="427e5-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="427e5-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="427e5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="427e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="427e5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="427e5-119">Request headers</span></span>
| <span data-ttu-id="427e5-120">Nome</span><span class="sxs-lookup"><span data-stu-id="427e5-120">Name</span></span>       | <span data-ttu-id="427e5-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="427e5-121">Type</span></span> | <span data-ttu-id="427e5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="427e5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="427e5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="427e5-123">Authorization</span></span>  | <span data-ttu-id="427e5-124">string</span><span class="sxs-lookup"><span data-stu-id="427e5-124">string</span></span>  | <span data-ttu-id="427e5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="427e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="427e5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="427e5-127">Request body</span></span>
<span data-ttu-id="427e5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="427e5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="427e5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="427e5-129">Response</span></span>

<span data-ttu-id="427e5-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="427e5-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="427e5-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="427e5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="427e5-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="427e5-133">Request</span></span>
<span data-ttu-id="427e5-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="427e5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="427e5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="427e5-135">Response</span></span>
<span data-ttu-id="427e5-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="427e5-136">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
