---
title: Atualizar CalendarGroup
description: Use esta API para criar um novo CalendarGroup.
ms.openlocfilehash: 2eb1f87a168a071822c90c778806bfc7e3569c03
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041042"
---
# <a name="create-calendargroup"></a><span data-ttu-id="34320-103">Atualizar CalendarGroup</span><span class="sxs-lookup"><span data-stu-id="34320-103">Create CalendarGroup</span></span>

> <span data-ttu-id="34320-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34320-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34320-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34320-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34320-106">Use esta API para criar um novo CalendarGroup.</span><span class="sxs-lookup"><span data-stu-id="34320-106">Use this API to create a new CalendarGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="34320-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="34320-107">Permissions</span></span>
<span data-ttu-id="34320-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34320-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34320-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34320-110">Permission type</span></span>      | <span data-ttu-id="34320-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34320-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34320-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34320-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34320-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34320-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="34320-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34320-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34320-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34320-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="34320-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34320-116">Application</span></span> | <span data-ttu-id="34320-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34320-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="34320-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34320-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendarGroups
```
## <a name="request-headers"></a><span data-ttu-id="34320-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34320-119">Request headers</span></span>
| <span data-ttu-id="34320-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34320-120">Header</span></span>       | <span data-ttu-id="34320-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34320-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34320-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34320-122">Authorization</span></span>  | <span data-ttu-id="34320-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34320-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="34320-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34320-125">Content-Type</span></span>  | <span data-ttu-id="34320-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34320-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34320-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34320-127">Request body</span></span>
<span data-ttu-id="34320-128">No corpo da solicitação, forneça uma representação JSON do objeto [CalendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="34320-128">In the request body, supply a JSON representation of [CalendarGroup](../resources/calendargroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="34320-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34320-129">Response</span></span>

<span data-ttu-id="34320-130">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34320-130">If successful, this method returns `201 Created` response code and [CalendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34320-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34320-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34320-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34320-132">Request</span></span>
<span data-ttu-id="34320-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34320-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendargroup_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendarGroups
Content-type: application/json
Content-length: 90

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value"
}
```
<span data-ttu-id="34320-134">No corpo da solicitação, forneça uma representação JSON do objeto [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="34320-134">In the request body, supply a JSON representation of [calendarGroup](../resources/calendargroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="34320-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="34320-135">Response</span></span>
<span data-ttu-id="34320-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34320-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "classId-value",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create CalendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
