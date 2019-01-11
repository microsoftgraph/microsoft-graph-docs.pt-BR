---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eec8a198c783a0c04ba1e20d73095701c471b5cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845665"
---
# <a name="delete-device"></a><span data-ttu-id="16f44-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="16f44-103">Delete device</span></span>

<span data-ttu-id="16f44-104">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="16f44-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="16f44-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="16f44-105">Permissions</span></span>
<span data-ttu-id="16f44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16f44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="16f44-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16f44-108">Permission type</span></span>      | <span data-ttu-id="16f44-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="16f44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16f44-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16f44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="16f44-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="16f44-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="16f44-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16f44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16f44-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16f44-113">Not supported.</span></span>    |
|<span data-ttu-id="16f44-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16f44-114">Application</span></span> | <span data-ttu-id="16f44-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16f44-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="16f44-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16f44-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="16f44-117">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="16f44-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="16f44-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16f44-118">Request headers</span></span>
| <span data-ttu-id="16f44-119">Nome</span><span class="sxs-lookup"><span data-stu-id="16f44-119">Name</span></span>       | <span data-ttu-id="16f44-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="16f44-120">Type</span></span> | <span data-ttu-id="16f44-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="16f44-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="16f44-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="16f44-122">Authorization</span></span>  | <span data-ttu-id="16f44-123">string</span><span class="sxs-lookup"><span data-stu-id="16f44-123">string</span></span>  | <span data-ttu-id="16f44-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16f44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="16f44-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16f44-126">Request body</span></span>
<span data-ttu-id="16f44-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="16f44-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="16f44-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f44-128">Response</span></span>

<span data-ttu-id="16f44-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16f44-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16f44-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16f44-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="16f44-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16f44-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="16f44-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="16f44-133">Response</span></span>

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
