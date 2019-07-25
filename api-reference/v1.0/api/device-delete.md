---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2da35ff5f76fb6e030f7cf02ba60bd6b754382fb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883523"
---
# <a name="delete-device"></a><span data-ttu-id="0eaef-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="0eaef-103">Delete device</span></span>

<span data-ttu-id="0eaef-104">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="0eaef-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="0eaef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0eaef-105">Permissions</span></span>
<span data-ttu-id="0eaef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0eaef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0eaef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0eaef-108">Permission type</span></span>      | <span data-ttu-id="0eaef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0eaef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0eaef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0eaef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0eaef-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0eaef-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0eaef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0eaef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0eaef-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0eaef-113">Not supported.</span></span>    |
|<span data-ttu-id="0eaef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0eaef-114">Application</span></span> | <span data-ttu-id="0eaef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0eaef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0eaef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0eaef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="0eaef-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="0eaef-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eaef-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0eaef-118">Request headers</span></span>
| <span data-ttu-id="0eaef-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0eaef-119">Name</span></span>       | <span data-ttu-id="0eaef-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0eaef-120">Type</span></span> | <span data-ttu-id="0eaef-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eaef-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0eaef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0eaef-122">Authorization</span></span>  | <span data-ttu-id="0eaef-123">string</span><span class="sxs-lookup"><span data-stu-id="0eaef-123">string</span></span>  | <span data-ttu-id="0eaef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0eaef-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0eaef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0eaef-126">Request body</span></span>
<span data-ttu-id="0eaef-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0eaef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eaef-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0eaef-128">Response</span></span>

<span data-ttu-id="0eaef-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0eaef-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eaef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0eaef-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0eaef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0eaef-132">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0eaef-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0eaef-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0eaef-134">C#</span><span class="sxs-lookup"><span data-stu-id="0eaef-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0eaef-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="0eaef-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0eaef-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0eaef-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0eaef-137">Java</span><span class="sxs-lookup"><span data-stu-id="0eaef-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0eaef-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0eaef-138">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
