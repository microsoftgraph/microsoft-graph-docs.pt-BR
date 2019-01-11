---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2b34cffbff6b3c627ed13d6e4b2917f6f36f4f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854569"
---
# <a name="delete-device"></a><span data-ttu-id="014de-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="014de-103">Delete device</span></span>

> <span data-ttu-id="014de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="014de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="014de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="014de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="014de-106">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="014de-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="014de-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="014de-107">Permissions</span></span>
<span data-ttu-id="014de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="014de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="014de-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="014de-110">Permission type</span></span>      | <span data-ttu-id="014de-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="014de-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="014de-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="014de-112">Delegated (work or school account)</span></span> | <span data-ttu-id="014de-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="014de-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="014de-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="014de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="014de-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="014de-115">Not supported.</span></span>    |
|<span data-ttu-id="014de-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="014de-116">Application</span></span> | <span data-ttu-id="014de-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="014de-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="014de-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="014de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="014de-119">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="014de-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="014de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="014de-120">Request headers</span></span>
| <span data-ttu-id="014de-121">Nome</span><span class="sxs-lookup"><span data-stu-id="014de-121">Name</span></span>       | <span data-ttu-id="014de-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="014de-122">Type</span></span> | <span data-ttu-id="014de-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="014de-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="014de-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="014de-124">Authorization</span></span>  | <span data-ttu-id="014de-125">string</span><span class="sxs-lookup"><span data-stu-id="014de-125">string</span></span>  | <span data-ttu-id="014de-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="014de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="014de-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="014de-128">Request body</span></span>
<span data-ttu-id="014de-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="014de-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="014de-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="014de-130">Response</span></span>

<span data-ttu-id="014de-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="014de-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="014de-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="014de-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="014de-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="014de-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="014de-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="014de-135">Response</span></span>

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
