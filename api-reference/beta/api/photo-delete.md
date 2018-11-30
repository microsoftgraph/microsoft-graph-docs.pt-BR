---
title: Excluir foto
description: Exclua uma foto.
ms.openlocfilehash: 3a227ceb503caf947786adfb35265755e6059b0a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038154"
---
# <a name="delete-photo"></a><span data-ttu-id="acefa-103">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="acefa-103">Delete photo</span></span>

> <span data-ttu-id="acefa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="acefa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acefa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="acefa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="acefa-106">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="acefa-106">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="acefa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="acefa-107">Permissions</span></span>
<span data-ttu-id="acefa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acefa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acefa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acefa-110">Permission type</span></span>      | <span data-ttu-id="acefa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="acefa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acefa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acefa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="acefa-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acefa-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="acefa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acefa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acefa-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="acefa-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="acefa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acefa-116">Application</span></span> | <span data-ttu-id="acefa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acefa-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="acefa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acefa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="acefa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acefa-119">Request headers</span></span>
| <span data-ttu-id="acefa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="acefa-120">Name</span></span>       | <span data-ttu-id="acefa-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="acefa-121">Type</span></span> | <span data-ttu-id="acefa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="acefa-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="acefa-123">if-match</span><span class="sxs-lookup"><span data-stu-id="acefa-123">if-match</span></span>  | <span data-ttu-id="acefa-124">string</span><span class="sxs-lookup"><span data-stu-id="acefa-124">string</span></span>  | <span data-ttu-id="acefa-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="acefa-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="acefa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="acefa-126">Authorization</span></span>  | <span data-ttu-id="acefa-127">string</span><span class="sxs-lookup"><span data-stu-id="acefa-127">string</span></span>  | <span data-ttu-id="acefa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="acefa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acefa-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acefa-130">Request body</span></span>
<span data-ttu-id="acefa-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acefa-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acefa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="acefa-132">Response</span></span>

<span data-ttu-id="acefa-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acefa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acefa-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acefa-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="acefa-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acefa-136">Request</span></span>
<span data-ttu-id="acefa-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="acefa-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="acefa-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="acefa-138">Response</span></span>
<span data-ttu-id="acefa-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acefa-139">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
