---
title: Listar calendários
description: 'Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico. '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 576defc97cfaf7b3d6924f522e6463fcb56907d7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526274"
---
# <a name="list-calendars"></a><span data-ttu-id="b5f14-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="b5f14-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5f14-104">Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="b5f14-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="b5f14-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5f14-105">Permissions</span></span>
<span data-ttu-id="b5f14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5f14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5f14-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5f14-108">Permission type</span></span>      | <span data-ttu-id="b5f14-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5f14-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5f14-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5f14-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5f14-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5f14-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b5f14-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5f14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5f14-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5f14-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="b5f14-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5f14-114">Application</span></span> | <span data-ttu-id="b5f14-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5f14-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5f14-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5f14-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b5f14-117">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="b5f14-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="b5f14-118">Os calendários do usuário no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="b5f14-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="b5f14-119">Os calendários do usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="b5f14-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5f14-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5f14-120">Optional query parameters</span></span>
<span data-ttu-id="b5f14-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5f14-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5f14-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5f14-122">Request headers</span></span>
| <span data-ttu-id="b5f14-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5f14-123">Header</span></span>       | <span data-ttu-id="b5f14-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b5f14-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b5f14-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5f14-125">Authorization</span></span>  | <span data-ttu-id="b5f14-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5f14-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b5f14-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5f14-128">Content-Type</span></span>   | <span data-ttu-id="b5f14-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b5f14-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5f14-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5f14-130">Request body</span></span>
<span data-ttu-id="b5f14-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5f14-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5f14-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5f14-132">Response</span></span>

<span data-ttu-id="b5f14-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5f14-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5f14-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5f14-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5f14-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5f14-135">Request</span></span>
<span data-ttu-id="b5f14-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5f14-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="b5f14-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5f14-137">Response</span></span>
<span data-ttu-id="b5f14-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5f14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "isDefaultCalendar": true,
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
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-calendars.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
