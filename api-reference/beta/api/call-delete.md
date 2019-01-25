---
title: Chamada Delete
description: Excluir ou desligar a uma chamada ativa.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ed4ae5c8fdd397541e015a31bc6ecee948f0ea0e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513232"
---
# <a name="delete-call"></a><span data-ttu-id="c2936-103">Chamada Delete</span><span class="sxs-lookup"><span data-stu-id="c2936-103">Delete call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2936-104">Excluir ou desligar a uma chamada ativa.</span><span class="sxs-lookup"><span data-stu-id="c2936-104">Delete or hang up an active call.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2936-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c2936-105">Permissions</span></span>

<span data-ttu-id="c2936-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2936-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c2936-108">Permission type</span></span> | <span data-ttu-id="c2936-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c2936-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="c2936-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c2936-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2936-111">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="c2936-111">Not Supported.</span></span>                         |
| <span data-ttu-id="c2936-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c2936-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2936-113">Não são suportados.</span><span class="sxs-lookup"><span data-stu-id="c2936-113">Not Supported.</span></span>                         |
| <span data-ttu-id="c2936-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c2936-114">Application</span></span>                            | <span data-ttu-id="c2936-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2936-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="c2936-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c2936-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /applications/{id}/calls/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c2936-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c2936-117">Request headers</span></span>
| <span data-ttu-id="c2936-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c2936-118">Name</span></span>          | <span data-ttu-id="c2936-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2936-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c2936-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c2936-120">Authorization</span></span> | <span data-ttu-id="c2936-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c2936-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2936-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c2936-123">Request body</span></span>
<span data-ttu-id="c2936-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c2936-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2936-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2936-125">Response</span></span>
<span data-ttu-id="c2936-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c2936-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2936-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c2936-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c2936-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c2936-129">Request</span></span>
<span data-ttu-id="c2936-130">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c2936-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete-call"
}-->
```http
DELETE https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="c2936-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c2936-131">Response</span></span>

> <span data-ttu-id="c2936-p104">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c2936-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

##### <a name="notification---terminating"></a><span data-ttu-id="c2936-134">Notificação - abortar</span><span class="sxs-lookup"><span data-stu-id="c2936-134">Notification - terminating</span></span>

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

##### <a name="notification---terminated"></a><span data-ttu-id="c2936-135">Notificação - terminada</span><span class="sxs-lookup"><span data-stu-id="c2936-135">Notification - terminated</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/call-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
