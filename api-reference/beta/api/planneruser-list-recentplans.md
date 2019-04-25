---
title: Listar recentPlans
description: Recupere uma lista de plannerPlans exibidos recentemente por um usuário. Você pode atualizar os planos exibidos recentemente atualizando o recurso plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: b4a8e25a31ceb17f85aef139378fa3e3e9058ab4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538697"
---
# <a name="list-recentplans"></a><span data-ttu-id="12476-104">Listar recentPlans</span><span class="sxs-lookup"><span data-stu-id="12476-104">List recentPlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12476-105">Recupere uma lista de [plannerPlans](../resources/plannerplan.md) exibidos recentemente por um usuário.</span><span class="sxs-lookup"><span data-stu-id="12476-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="12476-106">Você pode atualizar os planos exibidos recentemente [atualizando o recurso plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="12476-106">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="12476-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="12476-107">Permissions</span></span>
<span data-ttu-id="12476-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12476-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12476-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12476-110">Permission type</span></span>      | <span data-ttu-id="12476-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12476-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12476-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12476-112">Delegated (work or school account)</span></span> | <span data-ttu-id="12476-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="12476-113">Group.Read.All</span></span>    |
|<span data-ttu-id="12476-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12476-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12476-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12476-115">Not supported.</span></span>    |
|<span data-ttu-id="12476-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12476-116">Application</span></span> | <span data-ttu-id="12476-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12476-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12476-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12476-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="12476-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12476-119">Request headers</span></span>
| <span data-ttu-id="12476-120">Nome</span><span class="sxs-lookup"><span data-stu-id="12476-120">Name</span></span>      |<span data-ttu-id="12476-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="12476-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12476-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="12476-122">Authorization</span></span>  | <span data-ttu-id="12476-123">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="12476-123">Bearer {code}.</span></span> <span data-ttu-id="12476-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12476-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12476-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12476-125">Request body</span></span>
<span data-ttu-id="12476-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12476-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="12476-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="12476-127">Response</span></span>
<span data-ttu-id="12476-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [plannerPlan](../resources/plannerplan.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12476-128">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12476-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12476-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12476-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12476-130">Request</span></span>
<span data-ttu-id="12476-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12476-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="12476-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="12476-132">Response</span></span>
<span data-ttu-id="12476-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12476-133">The following is an example of the response.</span></span> 

><span data-ttu-id="12476-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12476-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-recentplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
