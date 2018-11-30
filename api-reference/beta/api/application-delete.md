---
title: Excluir aplicativo
description: Exclui um aplicativo.
ms.openlocfilehash: fc1f315de3e12574d51c58c56c1f37f39bdcd980
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035954"
---
# <a name="delete-application"></a><span data-ttu-id="3683d-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="3683d-103">Delete application</span></span>

> <span data-ttu-id="3683d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3683d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3683d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3683d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3683d-106">Exclui um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3683d-106">Deletes an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="3683d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3683d-107">Permissions</span></span>
<span data-ttu-id="3683d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3683d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3683d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3683d-110">Permission type</span></span>      | <span data-ttu-id="3683d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3683d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3683d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3683d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3683d-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3683d-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3683d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3683d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3683d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3683d-115">Not supported.</span></span>    |
|<span data-ttu-id="3683d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3683d-116">Application</span></span> | <span data-ttu-id="3683d-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3683d-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3683d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3683d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3683d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3683d-119">Request headers</span></span>
| <span data-ttu-id="3683d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3683d-120">Name</span></span>       | <span data-ttu-id="3683d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3683d-121">Type</span></span> | <span data-ttu-id="3683d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3683d-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3683d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3683d-123">Authorization</span></span>  | <span data-ttu-id="3683d-124">string</span><span class="sxs-lookup"><span data-stu-id="3683d-124">string</span></span>  | <span data-ttu-id="3683d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3683d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3683d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3683d-127">Request body</span></span>
<span data-ttu-id="3683d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3683d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3683d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3683d-129">Response</span></span>

<span data-ttu-id="3683d-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3683d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3683d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3683d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3683d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3683d-133">Request</span></span>
<span data-ttu-id="3683d-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3683d-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="3683d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3683d-135">Response</span></span>
<span data-ttu-id="3683d-136">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3683d-136">Here is an example of the response.</span></span> 
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
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->