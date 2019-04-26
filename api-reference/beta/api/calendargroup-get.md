---
title: Obter calendarGroup
description: Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e52d3191598c551edfdc095087b51e25bf0d4268
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322311"
---
# <a name="get-calendargroup"></a><span data-ttu-id="de683-103">Obter calendarGroup</span><span class="sxs-lookup"><span data-stu-id="de683-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de683-104">Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="de683-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de683-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="de683-105">Permissions</span></span>

<span data-ttu-id="de683-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de683-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de683-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de683-108">Permission type</span></span>                        | <span data-ttu-id="de683-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de683-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="de683-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de683-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de683-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de683-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="de683-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de683-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de683-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de683-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="de683-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de683-114">Application</span></span>                            | <span data-ttu-id="de683-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="de683-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="de683-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de683-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="de683-117">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="de683-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de683-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de683-118">Optional query parameters</span></span>

<span data-ttu-id="de683-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de683-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de683-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de683-120">Request headers</span></span>

| <span data-ttu-id="de683-121">Nome</span><span class="sxs-lookup"><span data-stu-id="de683-121">Name</span></span>          | <span data-ttu-id="de683-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="de683-122">Type</span></span>   | <span data-ttu-id="de683-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="de683-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="de683-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="de683-124">Authorization</span></span> | <span data-ttu-id="de683-125">string</span><span class="sxs-lookup"><span data-stu-id="de683-125">string</span></span> | <span data-ttu-id="de683-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de683-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de683-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de683-128">Request body</span></span>

<span data-ttu-id="de683-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de683-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de683-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="de683-130">Response</span></span>

<span data-ttu-id="de683-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de683-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de683-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de683-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="de683-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de683-133">Request</span></span>

<span data-ttu-id="de683-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de683-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="de683-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="de683-135">Response</span></span>

<span data-ttu-id="de683-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de683-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
