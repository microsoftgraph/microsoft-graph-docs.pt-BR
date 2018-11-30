---
title: Excluir contactFolder
description: Exclui uma contactFolder que não a padrão.
ms.openlocfilehash: dd1ed79981051a1fbbc362e8f586281aa2659b57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036929"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="26889-103">Excluir contactFolder</span><span class="sxs-lookup"><span data-stu-id="26889-103">Delete contactFolder</span></span>

> <span data-ttu-id="26889-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26889-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26889-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26889-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26889-106">Exclui uma contactFolder que não a padrão.</span><span class="sxs-lookup"><span data-stu-id="26889-106">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="26889-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="26889-107">Permissions</span></span>
<span data-ttu-id="26889-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26889-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26889-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26889-110">Permission type</span></span>      | <span data-ttu-id="26889-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="26889-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26889-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26889-112">Delegated (work or school account)</span></span> | <span data-ttu-id="26889-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26889-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="26889-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26889-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="26889-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26889-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="26889-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26889-116">Application</span></span> | <span data-ttu-id="26889-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26889-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="26889-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26889-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="26889-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26889-119">Request headers</span></span>
| <span data-ttu-id="26889-120">Nome</span><span class="sxs-lookup"><span data-stu-id="26889-120">Name</span></span>       | <span data-ttu-id="26889-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="26889-121">Type</span></span> | <span data-ttu-id="26889-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="26889-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="26889-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="26889-123">Authorization</span></span>  | <span data-ttu-id="26889-124">string</span><span class="sxs-lookup"><span data-stu-id="26889-124">string</span></span>  | <span data-ttu-id="26889-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26889-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="26889-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26889-127">Request body</span></span>
<span data-ttu-id="26889-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="26889-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="26889-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="26889-129">Response</span></span>

<span data-ttu-id="26889-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26889-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26889-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26889-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26889-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26889-133">Request</span></span>
<span data-ttu-id="26889-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26889-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="26889-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="26889-135">Response</span></span>
<span data-ttu-id="26889-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26889-136">Here is an example of the response.</span></span> 
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
