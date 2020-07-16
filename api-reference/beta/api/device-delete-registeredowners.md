---
title: Excluir registeredowners
description: Remover um usuário como proprietário registrado do dispositivo.
localization_priority: Normal
author: michaelrm97
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f958a1af94d74b9eee3db8f925ed1d6d9246617
ms.sourcegitcommit: 9c1abb1c87177da20e1f5bbf1fae8131ab7e4f16
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45146850"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="f5ba6-103">Excluir registeredOwner</span><span class="sxs-lookup"><span data-stu-id="f5ba6-103">Delete registeredOwner</span></span>

<span data-ttu-id="f5ba6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ba6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5ba6-105">Remover um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5ba6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5ba6-106">Permissions</span></span>

<span data-ttu-id="f5ba6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5ba6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5ba6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5ba6-109">Permission type</span></span>      | <span data-ttu-id="f5ba6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5ba6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5ba6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5ba6-111">Delegated (work or school account)</span></span> |<span data-ttu-id="f5ba6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5ba6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f5ba6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5ba6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5ba6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-114">Not supported.</span></span>    |
|<span data-ttu-id="f5ba6-115">Application</span><span class="sxs-lookup"><span data-stu-id="f5ba6-115">Application</span></span> | <span data-ttu-id="f5ba6-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5ba6-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="f5ba6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ba6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f5ba6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ba6-118">Request headers</span></span>
| <span data-ttu-id="f5ba6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f5ba6-119">Name</span></span>       | <span data-ttu-id="f5ba6-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5ba6-120">Type</span></span> | <span data-ttu-id="f5ba6-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ba6-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f5ba6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5ba6-122">Authorization</span></span>  | <span data-ttu-id="f5ba6-123">string</span><span class="sxs-lookup"><span data-stu-id="f5ba6-123">string</span></span>  | <span data-ttu-id="f5ba6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5ba6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ba6-126">Request body</span></span>
<span data-ttu-id="f5ba6-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5ba6-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ba6-128">Response</span></span>

<span data-ttu-id="f5ba6-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f5ba6-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5ba6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5ba6-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5ba6-131">Request</span></span>
<span data-ttu-id="f5ba6-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f5ba6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5ba6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredOwners/{id}/$ref
```

---

##### <a name="response"></a><span data-ttu-id="f5ba6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5ba6-134">Response</span></span>
<span data-ttu-id="f5ba6-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5ba6-135">Here is an example of the response.</span></span>
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
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
