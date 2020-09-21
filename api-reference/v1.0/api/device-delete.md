---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f2dc83df4d0c722968d926724aa093c7241bad05
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013353"
---
# <a name="delete-device"></a><span data-ttu-id="0974e-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="0974e-103">Delete device</span></span>

<span data-ttu-id="0974e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0974e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0974e-105">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="0974e-105">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="0974e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0974e-106">Permissions</span></span>
<span data-ttu-id="0974e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0974e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0974e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0974e-109">Permission type</span></span>      | <span data-ttu-id="0974e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0974e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0974e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0974e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0974e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0974e-112">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="0974e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0974e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0974e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0974e-114">Not supported.</span></span>    |
|<span data-ttu-id="0974e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0974e-115">Application</span></span> | <span data-ttu-id="0974e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0974e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0974e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0974e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="0974e-118">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="0974e-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0974e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0974e-119">Request headers</span></span>
| <span data-ttu-id="0974e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0974e-120">Name</span></span>       | <span data-ttu-id="0974e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0974e-121">Type</span></span> | <span data-ttu-id="0974e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0974e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0974e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0974e-123">Authorization</span></span>  | <span data-ttu-id="0974e-124">string</span><span class="sxs-lookup"><span data-stu-id="0974e-124">string</span></span>  | <span data-ttu-id="0974e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0974e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0974e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0974e-127">Request body</span></span>
<span data-ttu-id="0974e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0974e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0974e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0974e-129">Response</span></span>

<span data-ttu-id="0974e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0974e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0974e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0974e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0974e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0974e-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0974e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0974e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
# <a name="c"></a>[<span data-ttu-id="0974e-135">C#</span><span class="sxs-lookup"><span data-stu-id="0974e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0974e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0974e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0974e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0974e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0974e-138">Java</span><span class="sxs-lookup"><span data-stu-id="0974e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0974e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0974e-139">Response</span></span>

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

