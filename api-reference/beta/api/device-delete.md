---
title: Excluir dispositivo
description: Exclui um dispositivo registrado.
ms.openlocfilehash: 5635e183a2aebc11e95c5836076ad513075f50d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034018"
---
# <a name="delete-device"></a><span data-ttu-id="b8b94-103">Excluir dispositivo</span><span class="sxs-lookup"><span data-stu-id="b8b94-103">Delete device</span></span>

> <span data-ttu-id="b8b94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8b94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8b94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8b94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8b94-106">Exclui um dispositivo registrado.</span><span class="sxs-lookup"><span data-stu-id="b8b94-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8b94-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8b94-107">Permissions</span></span>
<span data-ttu-id="b8b94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8b94-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8b94-110">Permission type</span></span>      | <span data-ttu-id="b8b94-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8b94-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8b94-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8b94-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b8b94-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8b94-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="b8b94-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8b94-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8b94-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8b94-115">Not supported.</span></span>    |
|<span data-ttu-id="b8b94-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8b94-116">Application</span></span> | <span data-ttu-id="b8b94-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b8b94-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8b94-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8b94-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="b8b94-119">Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".</span><span class="sxs-lookup"><span data-stu-id="b8b94-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8b94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b94-120">Request headers</span></span>
| <span data-ttu-id="b8b94-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b8b94-121">Name</span></span>       | <span data-ttu-id="b8b94-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8b94-122">Type</span></span> | <span data-ttu-id="b8b94-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8b94-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8b94-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8b94-124">Authorization</span></span>  | <span data-ttu-id="b8b94-125">string</span><span class="sxs-lookup"><span data-stu-id="b8b94-125">string</span></span>  | <span data-ttu-id="b8b94-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8b94-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8b94-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b94-128">Request body</span></span>
<span data-ttu-id="b8b94-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8b94-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8b94-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8b94-130">Response</span></span>

<span data-ttu-id="b8b94-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8b94-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8b94-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8b94-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8b94-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b94-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="b8b94-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8b94-135">Response</span></span>

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