---
title: Lista favoritePlans
description: Recupere uma lista de plannerPlans que são marcados como favorito por um usuário. Você pode marcar um plano como favorito, atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c189b3a3a7ed6d36272c05e9614fd6d0327600d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519119"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="b0e3d-104">Lista favoritePlans</span><span class="sxs-lookup"><span data-stu-id="b0e3d-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0e3d-105">Recupere uma lista de [plannerPlans](../resources/plannerplan.md) que são marcados como favorito por um usuário.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="b0e3d-106">Você pode marcar um plano como favorito, [Atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="b0e3d-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0e3d-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0e3d-107">Permissions</span></span>
<span data-ttu-id="b0e3d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e3d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0e3d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0e3d-110">Permission type</span></span>      | <span data-ttu-id="b0e3d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0e3d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0e3d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0e3d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0e3d-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0e3d-113">Group.Read.All</span></span>    |
|<span data-ttu-id="b0e3d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0e3d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0e3d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-115">Not supported.</span></span>    |
|<span data-ttu-id="b0e3d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0e3d-116">Application</span></span> | <span data-ttu-id="b0e3d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0e3d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0e3d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b0e3d-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b0e3d-119">Optional query parameters</span></span>
<span data-ttu-id="b0e3d-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b0e3d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e3d-121">Request headers</span></span>
| <span data-ttu-id="b0e3d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="b0e3d-122">Name</span></span>      |<span data-ttu-id="b0e3d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0e3d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0e3d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0e3d-124">Authorization</span></span>  | <span data-ttu-id="b0e3d-p104">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e3d-127">Request body</span></span>
<span data-ttu-id="b0e3d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b0e3d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0e3d-129">Response</span></span>
<span data-ttu-id="b0e3d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b0e3d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0e3d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0e3d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e3d-132">Request</span></span>
<span data-ttu-id="b0e3d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="b0e3d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0e3d-134">Response</span></span>
<span data-ttu-id="b0e3d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-135">The following is an example of the response.</span></span> 

><span data-ttu-id="b0e3d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0e3d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
