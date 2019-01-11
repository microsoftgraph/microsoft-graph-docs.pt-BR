---
title: Obter calendarGroup
description: Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 399dcccbb264b8bd19e72b5e887236269581256a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824875"
---
# <a name="get-calendargroup"></a><span data-ttu-id="f0fa2-103">Obter calendarGroup</span><span class="sxs-lookup"><span data-stu-id="f0fa2-103">Get calendarGroup</span></span>

> <span data-ttu-id="f0fa2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0fa2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0fa2-106">Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-106">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0fa2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f0fa2-107">Permissions</span></span>

<span data-ttu-id="f0fa2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0fa2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0fa2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0fa2-110">Permission type</span></span>                        | <span data-ttu-id="f0fa2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f0fa2-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f0fa2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0fa2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0fa2-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0fa2-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="f0fa2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0fa2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0fa2-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0fa2-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="f0fa2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0fa2-116">Application</span></span>                            | <span data-ttu-id="f0fa2-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f0fa2-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="f0fa2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0fa2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f0fa2-119">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0fa2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f0fa2-120">Optional query parameters</span></span>

<span data-ttu-id="f0fa2-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0fa2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0fa2-122">Request headers</span></span>

| <span data-ttu-id="f0fa2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f0fa2-123">Name</span></span>          | <span data-ttu-id="f0fa2-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0fa2-124">Type</span></span>   | <span data-ttu-id="f0fa2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0fa2-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f0fa2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0fa2-126">Authorization</span></span> | <span data-ttu-id="f0fa2-127">string</span><span class="sxs-lookup"><span data-stu-id="f0fa2-127">string</span></span> | <span data-ttu-id="f0fa2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0fa2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0fa2-130">Request body</span></span>

<span data-ttu-id="f0fa2-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0fa2-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0fa2-132">Response</span></span>

<span data-ttu-id="f0fa2-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-133">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0fa2-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0fa2-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f0fa2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0fa2-135">Request</span></span>

<span data-ttu-id="f0fa2-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="f0fa2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0fa2-137">Response</span></span>

<span data-ttu-id="f0fa2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0fa2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
