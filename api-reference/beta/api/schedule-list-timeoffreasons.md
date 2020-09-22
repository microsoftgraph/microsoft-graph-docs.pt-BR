---
title: Listar timeOffReasons
description: Obtenha a lista de timeOffReasons em um cronograma.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 785f328c397539b13e96a5ec2dde8df4b5ca9c80
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047039"
---
# <a name="list-timeoffreasons"></a><span data-ttu-id="1434e-103">Listar timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="1434e-103">List timeOffReasons</span></span>

<span data-ttu-id="1434e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1434e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="1434e-105">Obtenha a lista de [timeOffReasons](../resources/timeoffreason.md) em um [cronograma](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="1434e-105">Get the list of [timeOffReasons](../resources/timeoffreason.md) in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1434e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1434e-106">Permissions</span></span>

<span data-ttu-id="1434e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1434e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1434e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1434e-109">Permission type</span></span>      | <span data-ttu-id="1434e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1434e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1434e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1434e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1434e-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1434e-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1434e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1434e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1434e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1434e-114">Not supported.</span></span>    |
|<span data-ttu-id="1434e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1434e-115">Application</span></span> | <span data-ttu-id="1434e-116">Schedule. Read. All *, Schedule. ReadWrite. All*</span><span class="sxs-lookup"><span data-stu-id="1434e-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="1434e-117">\***Importante:** As permissões de aplicativo estão atualmente em visualização privada apenas e não estão disponíveis para uso público.</span><span class="sxs-lookup"><span data-stu-id="1434e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="1434e-118">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="1434e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1434e-119">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="1434e-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1434e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1434e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="1434e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1434e-121">Request headers</span></span>

| <span data-ttu-id="1434e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1434e-122">Header</span></span>       | <span data-ttu-id="1434e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1434e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1434e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1434e-124">Authorization</span></span>  | <span data-ttu-id="1434e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1434e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1434e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1434e-127">Request body</span></span>
<span data-ttu-id="1434e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1434e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1434e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1434e-129">Response</span></span>

<span data-ttu-id="1434e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [timeOffReason](../resources/timeoffreason.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1434e-130">If successful, this method returns a `200 OK` response code and a collection of [timeOffReason](../resources/timeoffreason.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1434e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1434e-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1434e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1434e-132">Request</span></span>

<span data-ttu-id="1434e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1434e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1434e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1434e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-timeoffreasons"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
```
# <a name="c"></a>[<span data-ttu-id="1434e-135">C#</span><span class="sxs-lookup"><span data-stu-id="1434e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-timeoffreasons-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1434e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1434e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-timeoffreasons-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1434e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1434e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-timeoffreasons-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="1434e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1434e-138">Response</span></span>

<span data-ttu-id="1434e-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1434e-139">The following is an example of the response.</span></span> 

><span data-ttu-id="1434e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1434e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason",
  "isCollection": true
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
  ]
}
-->


