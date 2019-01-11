---
title: Criar calendário
description: Use esta API para criar um novo calendário em um grupo de calendários para um usuário.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 5cb13fc6259d21a752160b2a932f9a7c5b2330bd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819730"
---
# <a name="create-calendar"></a><span data-ttu-id="cc994-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="cc994-103">Create Calendar</span></span>

> <span data-ttu-id="cc994-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cc994-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc994-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cc994-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cc994-106">Use esta API para criar um novo calendário em um grupo de calendários para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="cc994-106">Use this API to create a new calendar in a calendar group for a [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc994-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc994-107">Permissions</span></span>

<span data-ttu-id="cc994-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc994-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc994-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc994-110">Permission type</span></span>                        | <span data-ttu-id="cc994-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc994-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="cc994-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc994-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc994-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc994-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="cc994-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc994-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc994-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc994-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="cc994-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc994-116">Application</span></span>                            | <span data-ttu-id="cc994-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc994-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="cc994-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc994-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="cc994-119">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="cc994-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="cc994-120">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="cc994-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a><span data-ttu-id="cc994-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc994-121">Request headers</span></span>

| <span data-ttu-id="cc994-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc994-122">Header</span></span>        | <span data-ttu-id="cc994-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cc994-123">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="cc994-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc994-124">Authorization</span></span> | <span data-ttu-id="cc994-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc994-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="cc994-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cc994-127">Content-Type</span></span>  | <span data-ttu-id="cc994-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc994-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc994-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc994-130">Request body</span></span>

<span data-ttu-id="cc994-131">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="cc994-131">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc994-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc994-132">Response</span></span>

<span data-ttu-id="cc994-133">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cc994-133">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc994-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc994-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cc994-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc994-135">Request</span></span>

<span data-ttu-id="cc994-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc994-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

<span data-ttu-id="cc994-137">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="cc994-137">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="cc994-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc994-138">Response</span></span>

<span data-ttu-id="cc994-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc994-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
