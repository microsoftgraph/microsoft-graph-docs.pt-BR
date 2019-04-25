---
title: Listar timeOffReasons
description: Obtenha a lista de timeOffReasons em um cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f91fab2b2a0acdd095b6c46168bd9971b40b667d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545779"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="cb199-103">Listar timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="cb199-103">List timeOffReasons</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="cb199-104">Obtenha a lista de [timeOffReasons](../resources/timeoffreason.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="cb199-104">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb199-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cb199-105">Permissions</span></span>

<span data-ttu-id="cb199-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb199-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cb199-108">Permission type</span></span>      | <span data-ttu-id="cb199-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cb199-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb199-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cb199-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb199-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb199-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb199-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cb199-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb199-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb199-113">Not supported.</span></span>    |
|<span data-ttu-id="cb199-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cb199-114">Application</span></span> | <span data-ttu-id="cb199-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cb199-115">Not supported.</span></span> |

> <span data-ttu-id="cb199-116">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="cb199-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="cb199-117">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="cb199-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="cb199-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cb199-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="cb199-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cb199-119">Request headers</span></span>

| <span data-ttu-id="cb199-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cb199-120">Header</span></span>       | <span data-ttu-id="cb199-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cb199-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb199-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cb199-122">Authorization</span></span>  | <span data-ttu-id="cb199-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cb199-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb199-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb199-125">Content-Type</span></span>  | <span data-ttu-id="cb199-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb199-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb199-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cb199-127">Request body</span></span>
<span data-ttu-id="cb199-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cb199-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb199-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb199-129">Response</span></span>

<span data-ttu-id="cb199-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cb199-130">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb199-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cb199-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="cb199-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cb199-132">Request</span></span>

<span data-ttu-id="cb199-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cb199-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
```

#### <a name="response"></a><span data-ttu-id="cb199-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cb199-134">Response</span></span>

<span data-ttu-id="cb199-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cb199-135">The following is an example of the response.</span></span> 

><span data-ttu-id="cb199-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cb199-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
      "createdDateTime": "2019-03-12T22:10:38.242Z",
      "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
      "displayName": "Vacation",
      "iconType": "plane",
      "isActive": true,
      "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
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
  "description": "Get the list of timeOffReason in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-list-timeoffreasons.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
