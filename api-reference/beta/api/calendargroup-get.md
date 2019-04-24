---
title: Obter calendarGroup
description: Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c5eb48f208a9f4a6e8fa0b6c6268722501b16d52
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461413"
---
# <a name="get-calendargroup"></a><span data-ttu-id="3ef1c-103">Obter calendarGroup</span><span class="sxs-lookup"><span data-stu-id="3ef1c-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ef1c-104">Recupera as propriedades e os relacionamentos de um objeto de grupo de calendários.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ef1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ef1c-105">Permissions</span></span>

<span data-ttu-id="3ef1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ef1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ef1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ef1c-108">Permission type</span></span>                        | <span data-ttu-id="3ef1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ef1c-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3ef1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ef1c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ef1c-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ef1c-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="3ef1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ef1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ef1c-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ef1c-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="3ef1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ef1c-114">Application</span></span>                            | <span data-ttu-id="3ef1c-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3ef1c-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3ef1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ef1c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3ef1c-117">Qualquer [calendarGroup](../resources/calendargroup.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ef1c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ef1c-118">Optional query parameters</span></span>

<span data-ttu-id="3ef1c-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ef1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef1c-120">Request headers</span></span>

| <span data-ttu-id="3ef1c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="3ef1c-121">Name</span></span>          | <span data-ttu-id="3ef1c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ef1c-122">Type</span></span>   | <span data-ttu-id="3ef1c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ef1c-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="3ef1c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ef1c-124">Authorization</span></span> | <span data-ttu-id="3ef1c-125">string</span><span class="sxs-lookup"><span data-stu-id="3ef1c-125">string</span></span> | <span data-ttu-id="3ef1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ef1c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef1c-128">Request body</span></span>

<span data-ttu-id="3ef1c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ef1c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef1c-130">Response</span></span>

<span data-ttu-id="3ef1c-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e um objeto [calendarGroup](../resources/calendargroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ef1c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3ef1c-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3ef1c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ef1c-133">Request</span></span>

<span data-ttu-id="3ef1c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="3ef1c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ef1c-135">Response</span></span>

<span data-ttu-id="3ef1c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ef1c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/calendargroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
