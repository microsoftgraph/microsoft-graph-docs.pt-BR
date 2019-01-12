---
title: Chamada Delete
description: Excluir ou desligar a uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 0163f7eee4933406999e283378f31d7f5aeb92b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946761"
---
# <a name="delete-call"></a><span data-ttu-id="e6b57-103">Chamada Delete</span><span class="sxs-lookup"><span data-stu-id="e6b57-103">Delete call</span></span>

> <span data-ttu-id="e6b57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6b57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6b57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6b57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6b57-106">Excluir ou desligar a uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="e6b57-106">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6b57-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="e6b57-107">Permissions</span></span>

<span data-ttu-id="e6b57-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6b57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6b57-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6b57-110">Permission type</span></span> | <span data-ttu-id="e6b57-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6b57-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e6b57-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6b57-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6b57-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="e6b57-113">Not Supported.</span></span>                         |
| <span data-ttu-id="e6b57-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6b57-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6b57-115">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="e6b57-115">Not Supported.</span></span>                         |
| <span data-ttu-id="e6b57-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6b57-116">Application</span></span>                            | <span data-ttu-id="e6b57-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e6b57-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e6b57-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6b57-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e6b57-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b57-119">Request headers</span></span>
| <span data-ttu-id="e6b57-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e6b57-120">Name</span></span>          | <span data-ttu-id="e6b57-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6b57-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e6b57-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6b57-122">Authorization</span></span> | <span data-ttu-id="e6b57-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6b57-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6b57-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b57-125">Request body</span></span>
<span data-ttu-id="e6b57-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6b57-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6b57-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6b57-127">Response</span></span>
<span data-ttu-id="e6b57-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6b57-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6b57-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6b57-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e6b57-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b57-131">Request</span></span>
<span data-ttu-id="e6b57-132">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6b57-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="e6b57-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6b57-133">Response</span></span>

> <span data-ttu-id="e6b57-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6b57-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="e6b57-136">Notificação - abortar</span><span class="sxs-lookup"><span data-stu-id="e6b57-136">Notification - terminating</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "updated",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminating"
      }
    }
  ]
}
```

##### <a name="notification---terminated"></a><span data-ttu-id="e6b57-137">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="e6b57-137">Notification - terminated</span></span>

```http
POST https://bot.contoso.com/api/calls
Authorization: Bearer <TOKEN>
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [
    {
      "changeType": "deleted",
      "resource": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "@odata.id": "/app/calls/57DAB8B1894C409AB240BD8BEAE78896",
        "@odata.etag": "W/\"5445\"",
        "state": "terminated",
        "terminationReason": "AppInitiated"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
