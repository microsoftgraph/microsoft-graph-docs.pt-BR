---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 49bffc1147735aeefcbdb541804fbff386f2c77f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917570"
---
# <a name="delete-device"></a><span data-ttu-id="42665-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="42665-103">Delete device</span></span>

<span data-ttu-id="42665-104">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="42665-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="42665-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="42665-105">Permissions</span></span>
<span data-ttu-id="42665-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="42665-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42665-108">Permission type</span></span>      | <span data-ttu-id="42665-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42665-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42665-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42665-110">Delegated (work or school account)</span></span> | <span data-ttu-id="42665-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="42665-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="42665-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42665-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42665-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42665-113">Not supported.</span></span>    |
|<span data-ttu-id="42665-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42665-114">Application</span></span> | <span data-ttu-id="42665-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42665-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42665-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42665-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="42665-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="42665-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="42665-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42665-118">Request headers</span></span>
| <span data-ttu-id="42665-119">Nome</span><span class="sxs-lookup"><span data-stu-id="42665-119">Name</span></span>       | <span data-ttu-id="42665-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="42665-120">Type</span></span> | <span data-ttu-id="42665-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="42665-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="42665-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="42665-122">Authorization</span></span>  | <span data-ttu-id="42665-123">string</span><span class="sxs-lookup"><span data-stu-id="42665-123">string</span></span>  | <span data-ttu-id="42665-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42665-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42665-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42665-126">Request body</span></span>
<span data-ttu-id="42665-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42665-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42665-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="42665-128">Response</span></span>

<span data-ttu-id="42665-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42665-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42665-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42665-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42665-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42665-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="42665-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="42665-133">Response</span></span>

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
