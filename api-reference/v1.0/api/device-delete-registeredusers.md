---
title: Excluir registeredUsers
description: Remover um usuário como um usuário registrado do dispositivo.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 40f510c0dd82efb47e0685c0432e2d3b42b2ce9d
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146713"
---
# <a name="delete-registereduser"></a><span data-ttu-id="4ea4f-103">Excluir registeredUser</span><span class="sxs-lookup"><span data-stu-id="4ea4f-103">Delete registeredUser</span></span>

<span data-ttu-id="4ea4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ea4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ea4f-105">Remover um usuário como um usuário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-105">Remove a user as a registered user of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ea4f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4ea4f-106">Permissions</span></span>

<span data-ttu-id="4ea4f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ea4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ea4f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4ea4f-109">Permission type</span></span>      | <span data-ttu-id="4ea4f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4ea4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ea4f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4ea4f-111">Delegated (work or school account)</span></span> |<span data-ttu-id="4ea4f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4ea4f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4ea4f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4ea4f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ea4f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-114">Not supported.</span></span>    |
|<span data-ttu-id="4ea4f-115">Application</span><span class="sxs-lookup"><span data-stu-id="4ea4f-115">Application</span></span> | <span data-ttu-id="4ea4f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ea4f-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="4ea4f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea4f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredUsers/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4ea4f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea4f-118">Request headers</span></span>
| <span data-ttu-id="4ea4f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4ea4f-119">Name</span></span>       | <span data-ttu-id="4ea4f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ea4f-120">Type</span></span> | <span data-ttu-id="4ea4f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ea4f-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4ea4f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4ea4f-122">Authorization</span></span>  | <span data-ttu-id="4ea4f-123">string</span><span class="sxs-lookup"><span data-stu-id="4ea4f-123">string</span></span>  | <span data-ttu-id="4ea4f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ea4f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea4f-126">Request body</span></span>
<span data-ttu-id="4ea4f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ea4f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea4f-128">Response</span></span>

<span data-ttu-id="4ea4f-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4ea4f-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4ea4f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ea4f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4ea4f-131">Request</span></span>
<span data-ttu-id="4ea4f-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4ea4f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ea4f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredusers"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers/{id}/$ref
```

---

##### <a name="response"></a><span data-ttu-id="4ea4f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4ea4f-134">Response</span></span>
<span data-ttu-id="4ea4f-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4ea4f-135">Here is an example of the response.</span></span>
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
  "description": "Delete registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
