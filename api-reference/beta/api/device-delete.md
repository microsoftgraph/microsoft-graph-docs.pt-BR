---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ee9bcfe46e0a931e47b4b4cbe0925fedf6bec7c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326096"
---
# <a name="delete-device"></a><span data-ttu-id="478ab-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="478ab-103">Delete device</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="478ab-104">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="478ab-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="478ab-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="478ab-105">Permissions</span></span>
<span data-ttu-id="478ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="478ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="478ab-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="478ab-108">Permission type</span></span>      | <span data-ttu-id="478ab-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="478ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="478ab-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="478ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="478ab-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="478ab-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="478ab-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="478ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="478ab-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="478ab-113">Not supported.</span></span>    |
|<span data-ttu-id="478ab-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="478ab-114">Application</span></span> | <span data-ttu-id="478ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="478ab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="478ab-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="478ab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="478ab-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="478ab-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="478ab-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="478ab-118">Request headers</span></span>
| <span data-ttu-id="478ab-119">Nome</span><span class="sxs-lookup"><span data-stu-id="478ab-119">Name</span></span>       | <span data-ttu-id="478ab-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="478ab-120">Type</span></span> | <span data-ttu-id="478ab-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="478ab-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="478ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="478ab-122">Authorization</span></span>  | <span data-ttu-id="478ab-123">string</span><span class="sxs-lookup"><span data-stu-id="478ab-123">string</span></span>  | <span data-ttu-id="478ab-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="478ab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="478ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="478ab-126">Request body</span></span>
<span data-ttu-id="478ab-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="478ab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="478ab-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="478ab-128">Response</span></span>

<span data-ttu-id="478ab-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="478ab-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="478ab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="478ab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="478ab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="478ab-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="478ab-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="478ab-133">Response</span></span>

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
  "suppressions": []
}
-->
