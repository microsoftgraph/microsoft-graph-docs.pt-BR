---
title: Atualizar CalendarGroup
description: Use esta API para criar um novo CalendarGroup.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 51d024b20cbf51067f4309eeb729aa9fc8162c53
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473119"
---
# <a name="create-calendargroup"></a><span data-ttu-id="f0ec3-103">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="f0ec3-103">Create CalendarGroup</span></span>

<span data-ttu-id="f0ec3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0ec3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0ec3-105">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="f0ec3-105">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0ec3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0ec3-106">Permissions</span></span>
<span data-ttu-id="f0ec3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0ec3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0ec3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0ec3-109">Permission type</span></span>      | <span data-ttu-id="f0ec3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0ec3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0ec3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0ec3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0ec3-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0ec3-112">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f0ec3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0ec3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ec3-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0ec3-114">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f0ec3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0ec3-115">Application</span></span> | <span data-ttu-id="f0ec3-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f0ec3-116">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0ec3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0ec3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendarGroups
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="f0ec3-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ec3-118">Request headers</span></span>
| <span data-ttu-id="f0ec3-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0ec3-119">Header</span></span>       | <span data-ttu-id="f0ec3-120">Valor</span><span class="sxs-lookup"><span data-stu-id="f0ec3-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f0ec3-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0ec3-121">Authorization</span></span>  | <span data-ttu-id="f0ec3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0ec3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f0ec3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f0ec3-124">Content-Type</span></span>  | <span data-ttu-id="f0ec3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0ec3-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f0ec3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ec3-126">Request body</span></span>
<span data-ttu-id="f0ec3-127">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f0ec3-127">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f0ec3-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0ec3-128">Response</span></span>

<span data-ttu-id="f0ec3-129">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0ec3-129">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0ec3-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0ec3-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0ec3-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0ec3-131">Request</span></span>
<span data-ttu-id="f0ec3-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0ec3-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups
Content-type: application/json

{
  "name": "Personal events"
}
```

<span data-ttu-id="f0ec3-133">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f0ec3-133">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
### <a name="response"></a><span data-ttu-id="f0ec3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0ec3-134">Response</span></span>
<span data-ttu-id="f0ec3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0ec3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('7d54cb02-aaa3-4016-9f9c-a4b49422dd9b')/calendarGroups/$entity",
    "id": "AAMkADIxYjJiYmIzLTFmNjYtNGNhMy0YOkcEEh3vhfAAAGgdFjAAA=",
    "name": "Personal events",
    "classId": "44288f7d-7710-4293-8c8e-36f310ed2e6a",
    "changeKey": "NreqLYgxdE2DpHBBId74XwAABn6y8Q=="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

