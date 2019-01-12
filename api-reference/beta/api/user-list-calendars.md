---
title: Listar calendários
description: 'Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico. '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e34c6acbcab5e5da4852d547038be6891806b4d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983517"
---
# <a name="list-calendars"></a><span data-ttu-id="fbcaa-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="fbcaa-103">List calendars</span></span>

> <span data-ttu-id="fbcaa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbcaa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fbcaa-106">Obtenha calendários de todos do usuário (propriedade de navegação `/calendars`), obtenha os calendários do grupo padrão de calendários ou de um grupo de calendários específico.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-106">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="fbcaa-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fbcaa-107">Permissions</span></span>
<span data-ttu-id="fbcaa-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbcaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbcaa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fbcaa-110">Permission type</span></span>      | <span data-ttu-id="fbcaa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fbcaa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbcaa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fbcaa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbcaa-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbcaa-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fbcaa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fbcaa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbcaa-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbcaa-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="fbcaa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbcaa-116">Application</span></span> | <span data-ttu-id="fbcaa-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fbcaa-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbcaa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fbcaa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="fbcaa-119">Calendários de todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-119">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="fbcaa-120">Os calendários do usuário no [calendarGroup](../resources/calendargroup.md) padrão.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-120">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="fbcaa-121">Os calendários do usuário em um [calendarGroup](../resources/calendargroup.md) específico.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-121">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fbcaa-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fbcaa-122">Optional query parameters</span></span>
<span data-ttu-id="fbcaa-123">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fbcaa-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fbcaa-124">Request headers</span></span>
| <span data-ttu-id="fbcaa-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fbcaa-125">Header</span></span>       | <span data-ttu-id="fbcaa-126">Valor</span><span class="sxs-lookup"><span data-stu-id="fbcaa-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbcaa-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="fbcaa-127">Authorization</span></span>  | <span data-ttu-id="fbcaa-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fbcaa-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fbcaa-130">Content-Type</span></span>   | <span data-ttu-id="fbcaa-131">application/json</span><span class="sxs-lookup"><span data-stu-id="fbcaa-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbcaa-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fbcaa-132">Request body</span></span>
<span data-ttu-id="fbcaa-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbcaa-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbcaa-134">Response</span></span>

<span data-ttu-id="fbcaa-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-135">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbcaa-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fbcaa-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbcaa-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbcaa-137">Request</span></span>
<span data-ttu-id="fbcaa-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="fbcaa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="fbcaa-139">Response</span></span>
<span data-ttu-id="fbcaa-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fbcaa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
