---
title: Criar calendário
description: Use esta API para criar um novo calendário em um grupo de calendários para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cc49f343904a973c0b24cf541754013bf222910b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003914"
---
# <a name="create-calendar"></a><span data-ttu-id="f30f7-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="f30f7-103">Create Calendar</span></span>

<span data-ttu-id="f30f7-104">Use esta API para criar um novo calendário em um grupo de calendários para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f30f7-104">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f30f7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f30f7-105">Permissions</span></span>

<span data-ttu-id="f30f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f30f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f30f7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f30f7-108">Permission type</span></span>                        | <span data-ttu-id="f30f7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f30f7-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f30f7-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f30f7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f30f7-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30f7-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="f30f7-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f30f7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f30f7-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30f7-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="f30f7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f30f7-114">Application</span></span>                            | <span data-ttu-id="f30f7-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30f7-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f30f7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f30f7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f30f7-117">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="f30f7-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="f30f7-118">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f30f7-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="f30f7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f7-119">Request headers</span></span>

| <span data-ttu-id="f30f7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f30f7-120">Header</span></span>        | <span data-ttu-id="f30f7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f30f7-121">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="f30f7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f30f7-122">Authorization</span></span> | <span data-ttu-id="f30f7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f30f7-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="f30f7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f30f7-125">Content-Type</span></span>  | <span data-ttu-id="f30f7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f30f7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f30f7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f7-128">Request body</span></span>

<span data-ttu-id="f30f7-129">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="f30f7-129">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f30f7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f30f7-130">Response</span></span>

<span data-ttu-id="f30f7-131">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f30f7-131">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f30f7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f30f7-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f30f7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f30f7-133">Request</span></span>

<span data-ttu-id="f30f7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f30f7-134">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f30f7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f30f7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars

Content-type: application/json

{
  "name": "Marketing calendar"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f30f7-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="f30f7-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="f30f7-137">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="f30f7-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f30f7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f30f7-138">Response</span></span>

<span data-ttu-id="f30f7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f30f7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
    "id": "AAMkADYCQM0GfRAAAcrRD-AAA=",
    "name": "Marketing calendar",
    "color": "auto",
    "changeKey": "4xTfgHLeDkOqYVAkDNBn0QAAHKl46A==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
        "name": "Adele Vance",
        "address": "adelev@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
