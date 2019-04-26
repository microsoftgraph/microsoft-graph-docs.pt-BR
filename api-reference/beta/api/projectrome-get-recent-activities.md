---
title: Obter atividades recentes do usuário
description: " API. O serviço consultará o historyItems mais recente e, em seguida, extrairá as atividades relacionadas. As atividades serão classificadas de acordo com a **LastModified** mais recente no **historyItem**. Isso significa que as atividades sem **historyItems** não serão incluídas na resposta. A permissão userActivity. ReadWrite. CreatedByApp também aplicará filtragem adicional à resposta, de modo que somente as atividades criadas por seu aplicativo serão retornadas. Essa filtragem do lado do servidor pode resultar em páginas vazias se o usuário for particularmente ativo e outros aplicativos tiverem criado atividades mais recentes. Para obter as atividades do aplicativo, use a propriedade **nextLink** para paginar."
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 464d57e5257b1e9c85796e72e4b8cbda732d4946
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337185"
---
# <a name="get-recent-user-activities"></a><span data-ttu-id="04bee-109">Obter atividades recentes do usuário</span><span class="sxs-lookup"><span data-stu-id="04bee-109">Get recent user activities</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04bee-110">Obter atividades recentes para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="04bee-110">Get recent activities for a given user.</span></span> <span data-ttu-id="04bee-111">Essa função OData tem alguns comportamentos padrão incluídos para que funcionem como uma API "mais recentemente usada".</span><span class="sxs-lookup"><span data-stu-id="04bee-111">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="04bee-112">O serviço consultará o [historyItems](../resources/projectrome-historyitem.md)mais recente e, em seguida, extrairá as atividades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="04bee-112">The service will query for the most recent [historyItems](../resources/projectrome-historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="04bee-113">As atividades serão classificadas de acordo com a **LastModified** mais recente no **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="04bee-113">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="04bee-114">Isso significa que as atividades sem **historyItems** não serão incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="04bee-114">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="04bee-115">A permissão userActivity. ReadWrite. CreatedByApp também aplicará filtragem adicional à resposta, de modo que somente as atividades criadas por seu aplicativo serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="04bee-115">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="04bee-116">Essa filtragem do lado do servidor pode resultar em páginas vazias se o usuário for particularmente ativo e outros aplicativos tiverem criado atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="04bee-116">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="04bee-117">Para obter as atividades do aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="04bee-117">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="04bee-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="04bee-118">Permissions</span></span>

<span data-ttu-id="04bee-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04bee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04bee-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04bee-121">Permission type</span></span>      | <span data-ttu-id="04bee-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04bee-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04bee-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04bee-123">Delegated (work or school account)</span></span> | <span data-ttu-id="04bee-124">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="04bee-124">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="04bee-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04bee-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04bee-126">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="04bee-126">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="04bee-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04bee-127">Application</span></span> | <span data-ttu-id="04bee-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04bee-128">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04bee-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04bee-129">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04bee-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="04bee-130">Optional query parameters</span></span>

<span data-ttu-id="04bee-131">Este método oferece suporte a alguns [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="04bee-131">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="04bee-132">Há suporte para os seguintes parâmetros de consulta:</span><span class="sxs-lookup"><span data-stu-id="04bee-132">The following query parameters are supported:</span></span>

- <span data-ttu-id="04bee-133">$expand da propriedade de navegação **historyItems** .</span><span class="sxs-lookup"><span data-stu-id="04bee-133">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="04bee-134">$Top limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="04bee-134">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="04bee-135">$filter na propriedade **lastModifiedDateTime** para **atividades** ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="04bee-135">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="04bee-136">Veja a seguir alguns exemplos de consultas suportadas com codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="04bee-136">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="04bee-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04bee-137">Request headers</span></span>

|<span data-ttu-id="04bee-138">Nome</span><span class="sxs-lookup"><span data-stu-id="04bee-138">Name</span></span> | <span data-ttu-id="04bee-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="04bee-139">Type</span></span> | <span data-ttu-id="04bee-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="04bee-140">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="04bee-141">Autorização</span><span class="sxs-lookup"><span data-stu-id="04bee-141">Authorization</span></span> | <span data-ttu-id="04bee-142">string</span><span class="sxs-lookup"><span data-stu-id="04bee-142">string</span></span> | <span data-ttu-id="04bee-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04bee-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04bee-145">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04bee-145">Request body</span></span>

<span data-ttu-id="04bee-146">Não especifique um corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04bee-146">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="04bee-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="04bee-147">Response</span></span>

<span data-ttu-id="04bee-148">Se bem-sucedido, este método retorna o `200 OK` código de resposta com as atividades recentes do usuário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04bee-148">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="04bee-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04bee-149">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04bee-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04bee-150">Request</span></span>

<span data-ttu-id="04bee-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="04bee-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="04bee-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="04bee-152">Response</span></span>

<span data-ttu-id="04bee-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="04bee-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
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
<!--
{
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
