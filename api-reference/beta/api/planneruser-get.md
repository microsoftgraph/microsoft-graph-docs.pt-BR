---
title: Obter plannerUser
description: 'Recupere as propriedades e os relacionamentos de um objeto plannerUser. As propriedades retornadas incluem os planos favoritos do usuário e os planos exibidos recentemente. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 0ac20564183c36d26440b4532a39413dff47bfb6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546790"
---
# <a name="get-planneruser"></a><span data-ttu-id="5ef77-104">Obter plannerUser</span><span class="sxs-lookup"><span data-stu-id="5ef77-104">Get plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ef77-105">Recupere as propriedades e os relacionamentos de um objeto [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="5ef77-105">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="5ef77-106">As propriedades retornadas incluem os planos favoritos do usuário e os planos exibidos recentemente.</span><span class="sxs-lookup"><span data-stu-id="5ef77-106">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="5ef77-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ef77-107">Permissions</span></span>
<span data-ttu-id="5ef77-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ef77-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef77-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ef77-110">Permission type</span></span>      | <span data-ttu-id="5ef77-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ef77-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ef77-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ef77-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ef77-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="5ef77-113">Group.Read.All</span></span>    |
|<span data-ttu-id="5ef77-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ef77-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ef77-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ef77-115">Not supported.</span></span>    |
|<span data-ttu-id="5ef77-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ef77-116">Application</span></span> | <span data-ttu-id="5ef77-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ef77-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ef77-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ef77-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="5ef77-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ef77-119">Request headers</span></span>
| <span data-ttu-id="5ef77-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5ef77-120">Name</span></span>      |<span data-ttu-id="5ef77-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef77-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ef77-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ef77-122">Authorization</span></span>  | <span data-ttu-id="5ef77-123">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="5ef77-123">Bearer {code}.</span></span> <span data-ttu-id="5ef77-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ef77-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ef77-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ef77-125">Request body</span></span>
<span data-ttu-id="5ef77-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ef77-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5ef77-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ef77-127">Response</span></span>
<span data-ttu-id="5ef77-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [plannerUser](../resources/planneruser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ef77-128">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ef77-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ef77-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ef77-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ef77-130">Request</span></span>
<span data-ttu-id="5ef77-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ef77-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="5ef77-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ef77-132">Response</span></span>
<span data-ttu-id="5ef77-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5ef77-133">The following is an example of the response.</span></span> 

><span data-ttu-id="5ef77-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ef77-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
