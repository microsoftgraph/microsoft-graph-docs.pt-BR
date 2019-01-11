---
title: Excluir foto
description: Exclua uma foto.
localization_priority: Normal
ms.openlocfilehash: 117f4acbf5a45d9db64ccc5d3fc0ccc4d1c64896
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829257"
---
# <a name="delete-photo"></a><span data-ttu-id="5a8fd-103">Excluir foto</span><span class="sxs-lookup"><span data-stu-id="5a8fd-103">Delete photo</span></span>

> <span data-ttu-id="5a8fd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a8fd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a8fd-106">Exclua uma foto.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-106">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a8fd-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a8fd-107">Permissions</span></span>
<span data-ttu-id="5a8fd-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a8fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a8fd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a8fd-110">Permission type</span></span>      | <span data-ttu-id="5a8fd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a8fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a8fd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a8fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5a8fd-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a8fd-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a8fd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a8fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a8fd-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a8fd-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="5a8fd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a8fd-116">Application</span></span> | <span data-ttu-id="5a8fd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a8fd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a8fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="5a8fd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a8fd-119">Request headers</span></span>
| <span data-ttu-id="5a8fd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5a8fd-120">Name</span></span>       | <span data-ttu-id="5a8fd-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a8fd-121">Type</span></span> | <span data-ttu-id="5a8fd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a8fd-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5a8fd-123">if-match</span><span class="sxs-lookup"><span data-stu-id="5a8fd-123">if-match</span></span>  | <span data-ttu-id="5a8fd-124">string</span><span class="sxs-lookup"><span data-stu-id="5a8fd-124">string</span></span>  | <span data-ttu-id="5a8fd-125">Se este cabeçalho de solicitação estiver incluso e a eTag (ou cTag) fornecida não corresponder à marca atual no item, uma resposta `412 Precondition Failed` é exibida e o item não será excluído.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="5a8fd-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a8fd-126">Authorization</span></span>  | <span data-ttu-id="5a8fd-127">string</span><span class="sxs-lookup"><span data-stu-id="5a8fd-127">string</span></span>  | <span data-ttu-id="5a8fd-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a8fd-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a8fd-130">Request body</span></span>
<span data-ttu-id="5a8fd-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a8fd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a8fd-132">Response</span></span>

<span data-ttu-id="5a8fd-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a8fd-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a8fd-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a8fd-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a8fd-136">Request</span></span>
<span data-ttu-id="5a8fd-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="5a8fd-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a8fd-138">Response</span></span>
<span data-ttu-id="5a8fd-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a8fd-139">Here is an example of the response.</span></span>
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
