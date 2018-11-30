---
title: Criar calendário
description: Use esta API para criar um novo Calendar para um usuário.
ms.openlocfilehash: 8ffa88331478d7bbbe1e94c87d58505041d63d41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006935"
---
# <a name="create-calendar"></a><span data-ttu-id="86ed5-103">Criar calendário</span><span class="sxs-lookup"><span data-stu-id="86ed5-103">Create Calendar</span></span>

<span data-ttu-id="86ed5-104">Use esta API para criar um novo Calendar para um [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="86ed5-104">Use this API to create a new calendar for a [user](../resources/user.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="86ed5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="86ed5-105">Permissions</span></span>
<span data-ttu-id="86ed5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86ed5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86ed5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86ed5-108">Permission type</span></span>      | <span data-ttu-id="86ed5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86ed5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86ed5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86ed5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86ed5-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86ed5-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="86ed5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86ed5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86ed5-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86ed5-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="86ed5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86ed5-114">Application</span></span> | <span data-ttu-id="86ed5-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86ed5-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="86ed5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86ed5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/calendars
```
## <a name="request-headers"></a><span data-ttu-id="86ed5-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86ed5-117">Request headers</span></span>
| <span data-ttu-id="86ed5-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86ed5-118">Header</span></span>       | <span data-ttu-id="86ed5-119">Valor</span><span class="sxs-lookup"><span data-stu-id="86ed5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86ed5-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="86ed5-120">Authorization</span></span>  | <span data-ttu-id="86ed5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86ed5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="86ed5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86ed5-123">Content-Type</span></span>  | <span data-ttu-id="86ed5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86ed5-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86ed5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86ed5-125">Request body</span></span>
<span data-ttu-id="86ed5-126">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="86ed5-126">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="86ed5-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ed5-127">Response</span></span>

<span data-ttu-id="86ed5-128">Se bem-sucedido, este método retorna o código de resposta `201 Created` e o objeto [calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86ed5-128">If successful, this method returns `201 Created` response code and [calendar](../resources/calendar.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86ed5-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86ed5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86ed5-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86ed5-130">Request</span></span>
<span data-ttu-id="86ed5-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86ed5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_calendar_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendars
Content-type: application/json

{
  "name": "Volunteer"
}
```
<span data-ttu-id="86ed5-132">No corpo da solicitação, forneça uma representação JSON do objeto [calendar](../resources/calendar.md).</span><span class="sxs-lookup"><span data-stu-id="86ed5-132">In the request body, supply a JSON representation of [calendar](../resources/calendar.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="86ed5-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="86ed5-133">Response</span></span>
<span data-ttu-id="86ed5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86ed5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#me/calendars/$entity",
    "@odata.id":"https://graph.microsoft.com/v1.0/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/calendars('AAMkADJmMVAAA=')",
    "id":"AAMkADJmMVAAA=",
    "name":"Volunteer",
    "color":"auto",
    "changeKey":"DxYSthXJXEWwAQSYQnXvIgAAIxGttg==",
    "canShare":true,
    "canViewPrivateItems":true,
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
