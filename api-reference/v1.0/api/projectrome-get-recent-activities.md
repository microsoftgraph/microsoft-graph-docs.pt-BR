---
title: Obter atividades recentes do usuário
description: " API. O serviço consultará o historyItems mais recente e, em seguida, extrairá as atividades relacionadas. As atividades serão classificadas de acordo com a **LastModified** mais recente no **historyItem**. Isso significa que as atividades sem **historyItems** não serão incluídas na resposta. A permissão UserActivity. ReadWrite. CreatedByApp também aplicará filtragem adicional à resposta, de modo que somente as atividades criadas por seu aplicativo serão retornadas. Essa filtragem do lado do servidor pode resultar em páginas vazias se o usuário for particularmente ativo e outros aplicativos tiverem criado atividades mais recentes. Para obter as atividades do aplicativo, use a propriedade **nextLink** para paginar."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 79818c371547b90719d2128ff806c875a7bd47fa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272727"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="0da83-109">Obter atividades recentes do usuário</span><span class="sxs-lookup"><span data-stu-id="0da83-109">Get recent user activities</span></span>

<span data-ttu-id="0da83-110">Obter atividades recentes para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="0da83-110">Get recent activities for a given user.</span></span> <span data-ttu-id="0da83-111">Essa função OData tem alguns comportamentos padrão incluídos para que funcionem como uma API "mais recentemente usada".</span><span class="sxs-lookup"><span data-stu-id="0da83-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="0da83-112">O serviço consultará o [historyItems](../resources/projectrome-historyitem.md)mais recente e, em seguida, extrairá as atividades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="0da83-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="0da83-113">As atividades serão classificadas de acordo com a **LastModified** mais recente no **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="0da83-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="0da83-114">Isso significa que as atividades sem **historyItems** não serão incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="0da83-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="0da83-115">A permissão UserActivity. ReadWrite. CreatedByApp também aplicará filtragem adicional à resposta, de modo que somente as atividades criadas por seu aplicativo serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="0da83-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="0da83-116">Essa filtragem do lado do servidor pode resultar em páginas vazias se o usuário for particularmente ativo e outros aplicativos tiverem criado atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="0da83-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="0da83-117">Para obter as atividades do aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="0da83-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="0da83-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="0da83-118">Permissions</span></span>

<span data-ttu-id="0da83-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0da83-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0da83-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0da83-121">Permission type</span></span>      | <span data-ttu-id="0da83-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0da83-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0da83-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0da83-123">Delegated (work or school account)</span></span> | <span data-ttu-id="0da83-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0da83-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0da83-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0da83-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0da83-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="0da83-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="0da83-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0da83-127">Application</span></span> | <span data-ttu-id="0da83-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0da83-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0da83-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0da83-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0da83-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0da83-130">Optional query parameters</span></span>

<span data-ttu-id="0da83-131">Este método oferece suporte a alguns [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0da83-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="0da83-132">Há suporte para os seguintes parâmetros de consulta:</span><span class="sxs-lookup"><span data-stu-id="0da83-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="0da83-133">$expand da propriedade de navegação **historyItems** .</span><span class="sxs-lookup"><span data-stu-id="0da83-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="0da83-134">$top limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="0da83-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="0da83-135">$filter na propriedade **lastModifiedDateTime** para **atividades** ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="0da83-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="0da83-136">Veja a seguir alguns exemplos de consultas suportadas com codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="0da83-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="0da83-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0da83-137">Request headers</span></span>

|<span data-ttu-id="0da83-138">Nome</span><span class="sxs-lookup"><span data-stu-id="0da83-138">Name</span></span> | <span data-ttu-id="0da83-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="0da83-139">Type</span></span> | <span data-ttu-id="0da83-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="0da83-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="0da83-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="0da83-141">Authorization</span></span> | <span data-ttu-id="0da83-142">string</span><span class="sxs-lookup"><span data-stu-id="0da83-142">string</span></span> | <span data-ttu-id="0da83-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0da83-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0da83-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0da83-145">Request body</span></span>

<span data-ttu-id="0da83-146">Não especifique um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0da83-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="0da83-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="0da83-147">Response</span></span>

<span data-ttu-id="0da83-148">Se bem-sucedido, este método retorna o `200 OK` código de resposta com as atividades recentes do usuário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0da83-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="0da83-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0da83-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0da83-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0da83-150">Request</span></span>

<span data-ttu-id="0da83-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0da83-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="0da83-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="0da83-152">Response</span></span>

<span data-ttu-id="0da83-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0da83-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0da83-154">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="0da83-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0da83-155">C#</span><span class="sxs-lookup"><span data-stu-id="0da83-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_recent_activities-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0da83-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="0da83-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_recent_activities-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0da83-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="0da83-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_recent_activities-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
