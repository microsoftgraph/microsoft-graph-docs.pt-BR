---
title: Obter atividades recentes do usuário
description: " API. O serviço consultará os historyItems mais recentes e, em seguida, puxará essas atividades relacionadas. As atividades serão ordenadas de acordo com o **últimoModified mais** recente no **historyItem**. Isso significa que as atividades **sem historyItems** não serão incluídas na resposta. A permissão UserActivity.ReadWrite.CreatedByApp também aplicará filtragem extra à resposta, para que somente as atividades criadas por seu aplicativo sejam retornadas. Essa filtragem do lado do servidor poderá resultar em páginas vazias se o usuário estiver particularmente ativo e outros aplicativos criarem atividades mais recentes. Para obter as atividades do aplicativo, use a **propriedade nextLink** para paginar."
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 8a6b72fbe2041faf909dc3a2429d8891c5859261
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292326"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="9d6a7-109">Obter atividades recentes do usuário</span><span class="sxs-lookup"><span data-stu-id="9d6a7-109">Get recent user activities</span></span>

<span data-ttu-id="9d6a7-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d6a7-110">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d6a7-111">Obter atividades recentes para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-111">Get recent activities for a given user.</span></span> <span data-ttu-id="9d6a7-112">Essa função OData tem alguns comportamentos padrão incluídos para fazê-la funcionar como uma API "usada mais recentemente".</span><span class="sxs-lookup"><span data-stu-id="9d6a7-112">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="9d6a7-113">O serviço consultará os [historyItems](../resources/projectrome-historyitem.md)mais recentes e, em seguida, puxará essas atividades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-113">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="9d6a7-114">As atividades serão ordenadas de acordo com o **últimoModified mais** recente no **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-114">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="9d6a7-115">Isso significa que as atividades **sem historyItems** não serão incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-115">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="9d6a7-116">A permissão UserActivity.ReadWrite.CreatedByApp também aplicará filtragem extra à resposta, para que somente as atividades criadas por seu aplicativo sejam retornadas.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-116">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="9d6a7-117">Essa filtragem do lado do servidor poderá resultar em páginas vazias se o usuário estiver particularmente ativo e outros aplicativos criarem atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-117">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="9d6a7-118">Para obter as atividades do aplicativo, use a **propriedade nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-118">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d6a7-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d6a7-119">Permissions</span></span>

<span data-ttu-id="9d6a7-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d6a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d6a7-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d6a7-122">Permission type</span></span>      | <span data-ttu-id="9d6a7-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d6a7-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d6a7-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d6a7-124">Delegated (work or school account)</span></span> | <span data-ttu-id="9d6a7-125">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9d6a7-125">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9d6a7-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d6a7-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d6a7-127">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="9d6a7-127">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="9d6a7-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d6a7-128">Application</span></span> | <span data-ttu-id="9d6a7-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d6a7-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d6a7-130">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d6a7-131">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d6a7-131">Optional query parameters</span></span>

<span data-ttu-id="9d6a7-132">Esse método dá suporte a alguns [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-132">This method supports some [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="9d6a7-133">Há suporte para os seguintes parâmetros de consulta:</span><span class="sxs-lookup"><span data-stu-id="9d6a7-133">The following query parameters are supported:</span></span>

- <span data-ttu-id="9d6a7-134">$expand para a **propriedade de navegação historyItems.**</span><span class="sxs-lookup"><span data-stu-id="9d6a7-134">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="9d6a7-135">$top limitar o número máximo de itens entre páginas.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-135">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="9d6a7-136">$filter na propriedade **lastModifiedDateTime** para **atividades** ou **historyItems**, se expandido.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-136">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="9d6a7-137">A seguir estão alguns exemplos de consultas com suporte com codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-137">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="9d6a7-138">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d6a7-138">Request headers</span></span>

|<span data-ttu-id="9d6a7-139">Nome</span><span class="sxs-lookup"><span data-stu-id="9d6a7-139">Name</span></span> | <span data-ttu-id="9d6a7-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d6a7-140">Type</span></span> | <span data-ttu-id="9d6a7-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d6a7-141">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="9d6a7-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d6a7-142">Authorization</span></span> | <span data-ttu-id="9d6a7-143">string</span><span class="sxs-lookup"><span data-stu-id="9d6a7-143">string</span></span> | <span data-ttu-id="9d6a7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6a7-146">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d6a7-146">Request body</span></span>

<span data-ttu-id="9d6a7-147">Não especifique um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-147">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="9d6a7-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d6a7-148">Response</span></span>

<span data-ttu-id="9d6a7-149">Se bem-sucedido, este método retorna `200 OK` o código de resposta com as atividades recentes do usuário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-149">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="9d6a7-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d6a7-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9d6a7-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d6a7-151">Request</span></span>

<span data-ttu-id="9d6a7-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9d6a7-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d6a7-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/activities/recent
```
# <a name="c"></a>[<span data-ttu-id="9d6a7-154">C#</span><span class="sxs-lookup"><span data-stu-id="9d6a7-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-recent-activities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d6a7-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d6a7-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-recent-activities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d6a7-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d6a7-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-recent-activities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d6a7-157">Java</span><span class="sxs-lookup"><span data-stu-id="9d6a7-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-recent-activities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9d6a7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d6a7-158">Response</span></span>

<span data-ttu-id="9d6a7-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9d6a7-159">The following is an example of the response.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->
