---
title: Listar calendarGroups
description: Obter os grupos de calendários do usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ddd31fa4867d1653906ac6c331b284d18f3daa45
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567904"
---
# <a name="list-calendargroups"></a><span data-ttu-id="c4560-103">Listar calendarGroups</span><span class="sxs-lookup"><span data-stu-id="c4560-103">List calendarGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4560-104">Obter os grupos de calendários do usuário.</span><span class="sxs-lookup"><span data-stu-id="c4560-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="c4560-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c4560-105">Permissions</span></span>
<span data-ttu-id="c4560-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4560-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4560-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c4560-108">Permission type</span></span>      | <span data-ttu-id="c4560-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c4560-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4560-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c4560-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4560-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4560-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c4560-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c4560-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4560-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4560-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="c4560-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c4560-114">Application</span></span> | <span data-ttu-id="c4560-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c4560-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4560-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c4560-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarGroups
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c4560-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c4560-117">Optional query parameters</span></span>
<span data-ttu-id="c4560-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c4560-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c4560-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4560-119">Request headers</span></span>
| <span data-ttu-id="c4560-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c4560-120">Header</span></span>       | <span data-ttu-id="c4560-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c4560-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4560-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c4560-122">Authorization</span></span>  | <span data-ttu-id="c4560-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c4560-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4560-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4560-125">Content-Type</span></span>  | <span data-ttu-id="c4560-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c4560-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4560-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c4560-127">Request body</span></span>
<span data-ttu-id="c4560-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c4560-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4560-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4560-129">Response</span></span>

<span data-ttu-id="c4560-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [CalendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c4560-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c4560-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c4560-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4560-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c4560-132">Request</span></span>
<span data-ttu-id="c4560-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c4560-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="c4560-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c4560-134">Response</span></span>
<span data-ttu-id="c4560-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c4560-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
