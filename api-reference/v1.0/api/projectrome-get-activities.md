---
title: Obtenha as atividades do usuário
description: Obtenha atividades para um determinado usuário. Diferentemente do **recente** função OData, atividades sem históricos serão retornadas. A permissão UserActivity.ReadWrite.CreatedByApp serão aplicadas a filtragem extra à resposta, para que apenas as atividades criadas pelo seu aplicativo são retornadas. A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é particularmente ativo e outros aplicativos criou atividades mais recentes. Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: dce6420e33a5d57eb78d8ea4842ed759ebcdd11c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971792"
---
# <a name="get-user-activities"></a><span data-ttu-id="ab867-107">Obtenha as atividades do usuário</span><span class="sxs-lookup"><span data-stu-id="ab867-107">Get user activities</span></span>

<span data-ttu-id="ab867-108">Obtenha atividades para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="ab867-108">Get activities for a given user.</span></span> <span data-ttu-id="ab867-109">Diferentemente do **recente** função OData, atividades sem históricos serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="ab867-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="ab867-110">A permissão UserActivity.ReadWrite.CreatedByApp serão aplicadas a filtragem extra à resposta, para que apenas as atividades criadas pelo seu aplicativo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="ab867-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="ab867-111">A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é particularmente ativo e outros aplicativos criou atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="ab867-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="ab867-112">Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="ab867-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab867-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="ab867-113">Permissions</span></span>

<span data-ttu-id="ab867-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab867-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab867-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab867-116">Permission type</span></span>      | <span data-ttu-id="ab867-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab867-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab867-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab867-118">Delegated (work or school account)</span></span> | <span data-ttu-id="ab867-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ab867-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ab867-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab867-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab867-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ab867-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ab867-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab867-122">Application</span></span> | <span data-ttu-id="ab867-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab867-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab867-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab867-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab867-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab867-125">Optional query parameters</span></span>

<span data-ttu-id="ab867-126">Este método oferece suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab867-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="ab867-127">Os parâmetros de consulta a seguir são suportados:</span><span class="sxs-lookup"><span data-stu-id="ab867-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="ab867-128">$expand para a propriedade de navegação **historyItems** .</span><span class="sxs-lookup"><span data-stu-id="ab867-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="ab867-129">$top para limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="ab867-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="ab867-130">$filter na propriedade **lastModifiedDateTime** para atividades ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="ab867-130">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="ab867-131">Eis alguns exemplos de consultas compatíveis com a codificação de URL:</span><span class="sxs-lookup"><span data-stu-id="ab867-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="ab867-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab867-132">Request headers</span></span>

|<span data-ttu-id="ab867-133">Nome</span><span class="sxs-lookup"><span data-stu-id="ab867-133">Name</span></span> | <span data-ttu-id="ab867-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab867-134">Type</span></span> | <span data-ttu-id="ab867-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab867-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ab867-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab867-136">Authorization</span></span> | <span data-ttu-id="ab867-137">string</span><span class="sxs-lookup"><span data-stu-id="ab867-137">string</span></span> | <span data-ttu-id="ab867-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab867-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab867-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab867-140">Request body</span></span>

<span data-ttu-id="ab867-141">Nenhum corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab867-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="ab867-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab867-142">Response</span></span>

<span data-ttu-id="ab867-143">Se tiver êxito, este método retornará o `200 OK` código de resposta com atividades do usuário para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ab867-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="ab867-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab867-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ab867-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab867-145">Request</span></span>

<span data-ttu-id="ab867-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab867-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="ab867-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab867-147">Response</span></span>

<span data-ttu-id="ab867-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ab867-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
