---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 16a2a2478d00a527f0c9e0d010b62db3e20b7da7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590996"
---
# <a name="delete-device"></a><span data-ttu-id="e8e23-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="e8e23-103">Delete device</span></span>

<span data-ttu-id="e8e23-104">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="e8e23-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8e23-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8e23-105">Permissions</span></span>
<span data-ttu-id="e8e23-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e8e23-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8e23-108">Permission type</span></span>      | <span data-ttu-id="e8e23-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8e23-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8e23-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8e23-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8e23-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8e23-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e8e23-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8e23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8e23-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e23-113">Not supported.</span></span>    |
|<span data-ttu-id="e8e23-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e23-114">Application</span></span> | <span data-ttu-id="e8e23-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e23-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8e23-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="e8e23-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="e8e23-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8e23-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e23-118">Request headers</span></span>
| <span data-ttu-id="e8e23-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e8e23-119">Name</span></span>       | <span data-ttu-id="e8e23-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e23-120">Type</span></span> | <span data-ttu-id="e8e23-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e23-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8e23-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8e23-122">Authorization</span></span>  | <span data-ttu-id="e8e23-123">string</span><span class="sxs-lookup"><span data-stu-id="e8e23-123">string</span></span>  | <span data-ttu-id="e8e23-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8e23-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8e23-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e23-126">Request body</span></span>
<span data-ttu-id="e8e23-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8e23-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8e23-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e23-128">Response</span></span>

<span data-ttu-id="e8e23-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8e23-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e23-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8e23-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8e23-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e23-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="e8e23-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e23-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e8e23-134">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="e8e23-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e8e23-135">Basic</span><span class="sxs-lookup"><span data-stu-id="e8e23-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_device-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8e23-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8e23-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_device-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
