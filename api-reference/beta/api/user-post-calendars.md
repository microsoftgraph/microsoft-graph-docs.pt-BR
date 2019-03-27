---
title: Criar calendário
description: Use esta API para criar um novo Calendar para um usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: afbb37d9394f2c08c94c6c8f41c56431e6938831
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869327"
---
# <a name="create-calendar"></a><span data-ttu-id="a05d2-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="a05d2-103">Create Calendar</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a05d2-104">Use esta API para criar um novo Calendar para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a05d2-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a05d2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a05d2-105">Permissions</span></span>
<span data-ttu-id="a05d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a05d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a05d2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a05d2-108">Permission type</span></span>      | <span data-ttu-id="a05d2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a05d2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a05d2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a05d2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a05d2-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a05d2-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a05d2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a05d2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a05d2-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a05d2-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a05d2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a05d2-114">Application</span></span> | <span data-ttu-id="a05d2-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a05d2-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a05d2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a05d2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="a05d2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a05d2-117">Request headers</span></span>
| <span data-ttu-id="a05d2-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a05d2-118">Header</span></span>       | <span data-ttu-id="a05d2-119">Valor</span><span class="sxs-lookup"><span data-stu-id="a05d2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a05d2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a05d2-120">Authorization</span></span>  | <span data-ttu-id="a05d2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a05d2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a05d2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a05d2-123">Content-Type</span></span>  | <span data-ttu-id="a05d2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a05d2-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a05d2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a05d2-125">Request body</span></span>
<span data-ttu-id="a05d2-126">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="a05d2-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a05d2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05d2-127">Response</span></span>

<span data-ttu-id="a05d2-128">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a05d2-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a05d2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a05d2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a05d2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a05d2-130">Request</span></span>
<span data-ttu-id="a05d2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a05d2-131">Here is an example of the request.</span></span>
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
<span data-ttu-id="a05d2-132">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="a05d2-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a05d2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a05d2-133">Response</span></span>
<span data-ttu-id="a05d2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a05d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-calendars.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
