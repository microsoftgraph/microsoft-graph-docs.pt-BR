---
title: Listar calendários
description: Recupera uma lista de calendários que pertencem a um grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 161b4ecd59cb95c1c2da2513357d5d74c8620dfc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941531"
---
# <a name="list-calendars"></a><span data-ttu-id="6dede-103">Listar calendários</span><span class="sxs-lookup"><span data-stu-id="6dede-103">List calendars</span></span>

> <span data-ttu-id="6dede-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6dede-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6dede-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6dede-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6dede-106">Recupera uma lista de calendários que pertencem a um grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="6dede-106">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dede-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="6dede-107">Permissions</span></span>

<span data-ttu-id="6dede-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dede-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6dede-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6dede-110">Permission type</span></span>                        | <span data-ttu-id="6dede-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6dede-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="6dede-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6dede-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6dede-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6dede-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="6dede-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6dede-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dede-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6dede-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="6dede-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6dede-116">Application</span></span>                            | <span data-ttu-id="6dede-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6dede-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="6dede-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6dede-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6dede-119">Um [calendarGroup](../resources/calendargroup.md) padrão do usuário.</span><span class="sxs-lookup"><span data-stu-id="6dede-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="6dede-120">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6dede-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6dede-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6dede-121">Optional query parameters</span></span>

<span data-ttu-id="6dede-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6dede-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dede-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6dede-123">Request headers</span></span>

| <span data-ttu-id="6dede-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6dede-124">Name</span></span>          | <span data-ttu-id="6dede-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6dede-125">Type</span></span>   | <span data-ttu-id="6dede-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6dede-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="6dede-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6dede-127">Authorization</span></span> | <span data-ttu-id="6dede-128">string</span><span class="sxs-lookup"><span data-stu-id="6dede-128">string</span></span> | <span data-ttu-id="6dede-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6dede-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6dede-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6dede-131">Request body</span></span>

<span data-ttu-id="6dede-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6dede-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dede-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dede-133">Response</span></span>

<span data-ttu-id="6dede-134">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Calendar](../resources/calendar.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6dede-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dede-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6dede-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6dede-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6dede-136">Request</span></span>

<span data-ttu-id="6dede-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6dede-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="6dede-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6dede-138">Response</span></span>

<span data-ttu-id="6dede-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6dede-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
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
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
