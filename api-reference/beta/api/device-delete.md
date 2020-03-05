---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4d449576de3514fc8e11c1ce89489e69a0dd8730
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435995"
---
# <a name="delete-device"></a><span data-ttu-id="1cee8-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="1cee8-103">Delete device</span></span>

<span data-ttu-id="1cee8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1cee8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cee8-105">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="1cee8-105">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cee8-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cee8-106">Permissions</span></span>
<span data-ttu-id="1cee8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cee8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1cee8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cee8-109">Permission type</span></span>      | <span data-ttu-id="1cee8-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cee8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1cee8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cee8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1cee8-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1cee8-112">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="1cee8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cee8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cee8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cee8-114">Not supported.</span></span>    |
|<span data-ttu-id="1cee8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cee8-115">Application</span></span> | <span data-ttu-id="1cee8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cee8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cee8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cee8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="1cee8-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="1cee8-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cee8-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cee8-119">Request headers</span></span>
| <span data-ttu-id="1cee8-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1cee8-120">Name</span></span>       | <span data-ttu-id="1cee8-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cee8-121">Type</span></span> | <span data-ttu-id="1cee8-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cee8-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1cee8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cee8-123">Authorization</span></span>  | <span data-ttu-id="1cee8-124">string</span><span class="sxs-lookup"><span data-stu-id="1cee8-124">string</span></span>  | <span data-ttu-id="1cee8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cee8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cee8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cee8-127">Request body</span></span>
<span data-ttu-id="1cee8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cee8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cee8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cee8-129">Response</span></span>

<span data-ttu-id="1cee8-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cee8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cee8-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cee8-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1cee8-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cee8-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1cee8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cee8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="1cee8-135">C#</span><span class="sxs-lookup"><span data-stu-id="1cee8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cee8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cee8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cee8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cee8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1cee8-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cee8-138">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
