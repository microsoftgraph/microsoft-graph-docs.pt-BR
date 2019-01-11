---
title: Listar CalendarGroups
description: Obter os grupos de calendários do usuário.
localization_priority: Normal
ms.openlocfilehash: 75b3465bb2aac69ee6a8f38678734f6c6dd3473b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825793"
---
# <a name="list-calendargroups"></a><span data-ttu-id="e6b1f-103">Listar CalendarGroups</span><span class="sxs-lookup"><span data-stu-id="e6b1f-103">List calendarGroups</span></span>

> <span data-ttu-id="e6b1f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6b1f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6b1f-106">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-106">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6b1f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6b1f-107">Permissions</span></span>
<span data-ttu-id="e6b1f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6b1f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6b1f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6b1f-110">Permission type</span></span>      | <span data-ttu-id="e6b1f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6b1f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6b1f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6b1f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6b1f-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6b1f-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e6b1f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6b1f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6b1f-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6b1f-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e6b1f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6b1f-116">Application</span></span> | <span data-ttu-id="e6b1f-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6b1f-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6b1f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6b1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6b1f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e6b1f-119">Optional query parameters</span></span>
<span data-ttu-id="e6b1f-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e6b1f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b1f-121">Request headers</span></span>
| <span data-ttu-id="e6b1f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6b1f-122">Header</span></span>       | <span data-ttu-id="e6b1f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e6b1f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6b1f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6b1f-124">Authorization</span></span>  | <span data-ttu-id="e6b1f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e6b1f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6b1f-127">Content-Type</span></span>  | <span data-ttu-id="e6b1f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e6b1f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6b1f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b1f-129">Request body</span></span>
<span data-ttu-id="e6b1f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6b1f-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6b1f-131">Response</span></span>

<span data-ttu-id="e6b1f-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-132">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6b1f-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6b1f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6b1f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6b1f-134">Request</span></span>
<span data-ttu-id="e6b1f-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="e6b1f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6b1f-136">Response</span></span>
<span data-ttu-id="e6b1f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6b1f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
