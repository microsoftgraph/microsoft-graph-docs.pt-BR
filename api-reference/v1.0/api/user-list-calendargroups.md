---
title: Listar CalendarGroups
description: Obter os grupos de calendários do usuário.
ms.openlocfilehash: 5afdac039ad4e03eb61776c5a3eed92fee2bd577
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003878"
---
# <a name="list-calendargroups"></a><span data-ttu-id="eba64-103">Listar CalendarGroups</span><span class="sxs-lookup"><span data-stu-id="eba64-103">List calendarGroups</span></span>

<span data-ttu-id="eba64-104">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="eba64-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="eba64-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="eba64-105">Permissions</span></span>
<span data-ttu-id="eba64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eba64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eba64-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eba64-108">Permission type</span></span>      | <span data-ttu-id="eba64-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eba64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eba64-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eba64-110">Delegated (work or school account)</span></span> | <span data-ttu-id="eba64-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba64-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eba64-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eba64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eba64-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba64-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="eba64-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eba64-114">Application</span></span> | <span data-ttu-id="eba64-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eba64-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="eba64-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eba64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="eba64-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="eba64-117">Optional query parameters</span></span>
<span data-ttu-id="eba64-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="eba64-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="eba64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eba64-119">Request headers</span></span>
| <span data-ttu-id="eba64-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eba64-120">Header</span></span>       | <span data-ttu-id="eba64-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eba64-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eba64-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eba64-122">Authorization</span></span>  | <span data-ttu-id="eba64-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eba64-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eba64-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eba64-125">Content-Type</span></span>  | <span data-ttu-id="eba64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eba64-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eba64-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eba64-127">Request body</span></span>
<span data-ttu-id="eba64-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eba64-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eba64-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba64-129">Response</span></span>

<span data-ttu-id="eba64-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eba64-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eba64-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eba64-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eba64-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eba64-132">Request</span></span>
<span data-ttu-id="eba64-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eba64-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="eba64-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="eba64-134">Response</span></span>
<span data-ttu-id="eba64-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eba64-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
