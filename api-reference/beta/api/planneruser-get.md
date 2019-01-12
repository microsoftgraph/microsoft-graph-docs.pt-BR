---
title: Obter plannerUser
description: 'Recupere as propriedades e relacionamentos de um objeto plannerUser. As propriedades retornadas incluem planos de favoritos do usuário e visualizados recentemente planos. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 742d29d65c5d80db96c8cff199e25465f7a80dd7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915988"
---
# <a name="get-planneruser"></a><span data-ttu-id="7e049-104">Obter plannerUser</span><span class="sxs-lookup"><span data-stu-id="7e049-104">Get plannerUser</span></span>

> <span data-ttu-id="7e049-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e049-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e049-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e049-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e049-107">Recupere as propriedades e relacionamentos de um objeto [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="7e049-107">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="7e049-108">As propriedades retornadas incluem planos de favoritos do usuário e visualizados recentemente planos.</span><span class="sxs-lookup"><span data-stu-id="7e049-108">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="7e049-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e049-109">Permissions</span></span>
<span data-ttu-id="7e049-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e049-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e049-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e049-112">Permission type</span></span>      | <span data-ttu-id="7e049-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e049-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e049-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e049-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7e049-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e049-115">Group.Read.All</span></span>    |
|<span data-ttu-id="7e049-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e049-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e049-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e049-117">Not supported.</span></span>    |
|<span data-ttu-id="7e049-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e049-118">Application</span></span> | <span data-ttu-id="7e049-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e049-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e049-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e049-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="7e049-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e049-121">Request headers</span></span>
| <span data-ttu-id="7e049-122">Nome</span><span class="sxs-lookup"><span data-stu-id="7e049-122">Name</span></span>      |<span data-ttu-id="7e049-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e049-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7e049-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e049-124">Authorization</span></span>  | <span data-ttu-id="7e049-p105">Portador {código}. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e049-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e049-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e049-127">Request body</span></span>
<span data-ttu-id="7e049-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e049-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7e049-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e049-129">Response</span></span>
<span data-ttu-id="7e049-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [plannerUser](../resources/planneruser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e049-130">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e049-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e049-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e049-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e049-132">Request</span></span>
<span data-ttu-id="7e049-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e049-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="7e049-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e049-134">Response</span></span>
<span data-ttu-id="7e049-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7e049-135">The following is an example of the response.</span></span> 

><span data-ttu-id="7e049-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e049-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
