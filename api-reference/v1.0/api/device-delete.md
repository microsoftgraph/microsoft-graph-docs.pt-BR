---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
ms.openlocfilehash: 9e694eb23e6559e84fb26e549f867b9affb8a1c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005769"
---
# <a name="delete-device"></a><span data-ttu-id="e8a5e-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="e8a5e-103">Delete device</span></span>

<span data-ttu-id="e8a5e-104">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="e8a5e-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a5e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8a5e-105">Permissions</span></span>
<span data-ttu-id="e8a5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e8a5e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8a5e-108">Permission type</span></span>      | <span data-ttu-id="e8a5e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8a5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8a5e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8a5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8a5e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e8a5e-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e8a5e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8a5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a5e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8a5e-113">Not supported.</span></span>    |
|<span data-ttu-id="e8a5e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8a5e-114">Application</span></span> | <span data-ttu-id="e8a5e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8a5e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8a5e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a5e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="e8a5e-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="e8a5e-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8a5e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a5e-118">Request headers</span></span>
| <span data-ttu-id="e8a5e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e8a5e-119">Name</span></span>       | <span data-ttu-id="e8a5e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8a5e-120">Type</span></span> | <span data-ttu-id="e8a5e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8a5e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e8a5e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8a5e-122">Authorization</span></span>  | <span data-ttu-id="e8a5e-123">string</span><span class="sxs-lookup"><span data-stu-id="e8a5e-123">string</span></span>  | <span data-ttu-id="e8a5e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8a5e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8a5e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a5e-126">Request body</span></span>
<span data-ttu-id="e8a5e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8a5e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a5e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8a5e-128">Response</span></span>

<span data-ttu-id="e8a5e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8a5e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8a5e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8a5e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8a5e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a5e-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="e8a5e-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8a5e-133">Response</span></span>

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
  "tocPath": ""
}-->
