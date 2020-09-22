---
title: Obter plannerUser
description: 'Recupere as propriedades e relações de um objeto plannerUser. As propriedades retornadas incluem os planos favoritos do usuário e os planos exibidos recentemente. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 972ce36307cefbc528d3efed5367a93a79926fb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095722"
---
# <a name="get-planneruser"></a><span data-ttu-id="7b857-104">Obter plannerUser</span><span class="sxs-lookup"><span data-stu-id="7b857-104">Get plannerUser</span></span>

<span data-ttu-id="7b857-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b857-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b857-106">Recupere as propriedades e os relacionamentos de um objeto [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="7b857-106">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="7b857-107">As propriedades retornadas incluem os planos favoritos do usuário e os planos exibidos recentemente.</span><span class="sxs-lookup"><span data-stu-id="7b857-107">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="7b857-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="7b857-108">Permissions</span></span>
<span data-ttu-id="7b857-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b857-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b857-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b857-111">Permission type</span></span>      | <span data-ttu-id="7b857-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7b857-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b857-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b857-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7b857-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b857-114">Group.Read.All</span></span>    |
|<span data-ttu-id="7b857-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b857-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b857-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b857-116">Not supported.</span></span>    |
|<span data-ttu-id="7b857-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b857-117">Application</span></span> | <span data-ttu-id="7b857-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b857-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b857-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b857-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="7b857-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b857-120">Request headers</span></span>
| <span data-ttu-id="7b857-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7b857-121">Name</span></span>      |<span data-ttu-id="7b857-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b857-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7b857-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b857-123">Authorization</span></span>  | <span data-ttu-id="7b857-124">Portador {código}.</span><span class="sxs-lookup"><span data-stu-id="7b857-124">Bearer {code}.</span></span> <span data-ttu-id="7b857-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b857-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b857-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b857-126">Request body</span></span>
<span data-ttu-id="7b857-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b857-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7b857-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b857-128">Response</span></span>
<span data-ttu-id="7b857-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [plannerUser](../resources/planneruser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b857-129">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7b857-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b857-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b857-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b857-131">Request</span></span>
<span data-ttu-id="7b857-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b857-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="7b857-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b857-133">Response</span></span>
<span data-ttu-id="7b857-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7b857-134">The following is an example of the response.</span></span> 

><span data-ttu-id="7b857-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b857-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->


