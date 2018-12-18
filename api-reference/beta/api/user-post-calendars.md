---
title: Criar calendário
description: Use esta API para criar um novo Calendar para um usuário.
author: dkershaw10
ms.openlocfilehash: 320a34a22db3e8467af5c30c79ce41c6d18fc05b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339925"
---
# <a name="create-calendar"></a><span data-ttu-id="274b5-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="274b5-103">Create Calendar</span></span>

> <span data-ttu-id="274b5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="274b5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="274b5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="274b5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="274b5-106">Use esta API para criar um novo Calendar para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="274b5-106">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="274b5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="274b5-107">Permissions</span></span>
<span data-ttu-id="274b5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="274b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="274b5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="274b5-110">Permission type</span></span>      | <span data-ttu-id="274b5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="274b5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="274b5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="274b5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="274b5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274b5-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="274b5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="274b5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="274b5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274b5-115">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="274b5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="274b5-116">Application</span></span> | <span data-ttu-id="274b5-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="274b5-117">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="274b5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="274b5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="274b5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="274b5-119">Request headers</span></span>
| <span data-ttu-id="274b5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="274b5-120">Header</span></span>       | <span data-ttu-id="274b5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="274b5-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="274b5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="274b5-122">Authorization</span></span>  | <span data-ttu-id="274b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="274b5-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="274b5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="274b5-125">Content-Type</span></span>  | <span data-ttu-id="274b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="274b5-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="274b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="274b5-127">Request body</span></span>
<span data-ttu-id="274b5-128">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="274b5-128">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="274b5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="274b5-129">Response</span></span>

<span data-ttu-id="274b5-130">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="274b5-130">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="274b5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="274b5-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="274b5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="274b5-132">Request</span></span>
<span data-ttu-id="274b5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="274b5-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}

```
<span data-ttu-id="274b5-134">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="274b5-134">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="274b5-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="274b5-135">Response</span></span>
<span data-ttu-id="274b5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="274b5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "isDefaultCalendar":false,
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
    "hexColor": "",
    "isShared":false,
    "isSharedWithMe":false,
    "canEdit":true,
    "owner":{
        "name":"Samantha Booth",
        "address":"samanthab@adatum.onmicrosoft.com"
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
  "tocPath": ""
}-->