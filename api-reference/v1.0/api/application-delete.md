---
title: Excluir aplicativo
description: Excluir um objeto Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ecaafbaaa8558d8e9d86d45a75f824272fb6a14
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939730"
---
# <a name="delete-application"></a><span data-ttu-id="3cdc3-103">Excluir aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cdc3-103">Delete application</span></span>

<span data-ttu-id="3cdc3-104">Excluir um objeto [Application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="3cdc3-104">Delete an [application](../resources/application.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cdc3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cdc3-105">Permissions</span></span>
<span data-ttu-id="3cdc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cdc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cdc3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cdc3-108">Permission type</span></span>      | <span data-ttu-id="3cdc3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cdc3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cdc3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cdc3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3cdc3-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cdc3-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3cdc3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cdc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cdc3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cdc3-113">Not supported.</span></span>    |
|<span data-ttu-id="3cdc3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cdc3-114">Application</span></span> | <span data-ttu-id="3cdc3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cdc3-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cdc3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cdc3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /applications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3cdc3-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cdc3-117">Request headers</span></span>
| <span data-ttu-id="3cdc3-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3cdc3-118">Name</span></span>       | <span data-ttu-id="3cdc3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cdc3-119">Type</span></span> | <span data-ttu-id="3cdc3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cdc3-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cdc3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cdc3-121">Authorization</span></span>  | <span data-ttu-id="3cdc3-122">string</span><span class="sxs-lookup"><span data-stu-id="3cdc3-122">string</span></span>  | <span data-ttu-id="3cdc3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cdc3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cdc3-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cdc3-125">Request body</span></span>
<span data-ttu-id="3cdc3-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cdc3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cdc3-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cdc3-127">Response</span></span>

<span data-ttu-id="3cdc3-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cdc3-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cdc3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cdc3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cdc3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cdc3-131">Request</span></span>
<span data-ttu-id="3cdc3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cdc3-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_application"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}
```

##### <a name="response"></a><span data-ttu-id="3cdc3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cdc3-133">Response</span></span>
<span data-ttu-id="3cdc3-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cdc3-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
