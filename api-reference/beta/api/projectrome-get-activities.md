---
title: Obtenha as atividades do usuário
description: Obtenha atividades para um determinado usuário. Diferentemente do **recente** função OData, atividades sem históricos serão retornadas. A permissão UserActivity.ReadWrite.CreatedByApp serão aplicadas a filtragem extra à resposta, para que apenas as atividades criadas pelo seu aplicativo são retornadas. A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é particularmente ativo e outros aplicativos criou atividades mais recentes. Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.
localization_priority: Normal
ms.openlocfilehash: 8106d1c2cb740033fd81a21068aba5a15fd1b1b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809370"
---
# <a name="get-user-activities"></a><span data-ttu-id="b3c5e-107">Obtenha as atividades do usuário</span><span class="sxs-lookup"><span data-stu-id="b3c5e-107">Get user activities</span></span>

> <span data-ttu-id="b3c5e-108">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3c5e-109">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3c5e-110">Obtenha atividades para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-110">Get activities for a given user.</span></span> <span data-ttu-id="b3c5e-111">Diferentemente do **recente** função OData, atividades sem históricos serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-111">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="b3c5e-112">A permissão UserActivity.ReadWrite.CreatedByApp serão aplicadas a filtragem extra à resposta, para que apenas as atividades criadas pelo seu aplicativo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-112">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="b3c5e-113">A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é particularmente ativo e outros aplicativos criou atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-113">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="b3c5e-114">Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-114">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3c5e-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="b3c5e-115">Permissions</span></span>

<span data-ttu-id="b3c5e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3c5e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3c5e-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3c5e-118">Permission type</span></span>      | <span data-ttu-id="b3c5e-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3c5e-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3c5e-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3c5e-120">Delegated (work or school account)</span></span> | <span data-ttu-id="b3c5e-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b3c5e-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b3c5e-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3c5e-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3c5e-123">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b3c5e-123">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b3c5e-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3c5e-124">Application</span></span> | <span data-ttu-id="b3c5e-125">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3c5e-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3c5e-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3c5e-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3c5e-127">Optional query parameters</span></span>

<span data-ttu-id="b3c5e-128">Este método oferece suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-128">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="b3c5e-129">Os parâmetros de consulta a seguir são suportados:</span><span class="sxs-lookup"><span data-stu-id="b3c5e-129">The following query parameters are supported:</span></span>

- <span data-ttu-id="b3c5e-130">$expand para a propriedade de navegação **historyItems** .</span><span class="sxs-lookup"><span data-stu-id="b3c5e-130">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="b3c5e-131">$top para limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-131">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="b3c5e-132">$filter na propriedade **lastModifiedDateTime** para **atividades** ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-132">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="b3c5e-133">Eis alguns exemplos de consultas compatíveis com a codificação de URL:</span><span class="sxs-lookup"><span data-stu-id="b3c5e-133">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="b3c5e-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3c5e-134">Request headers</span></span>

|<span data-ttu-id="b3c5e-135">Nome</span><span class="sxs-lookup"><span data-stu-id="b3c5e-135">Name</span></span> | <span data-ttu-id="b3c5e-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3c5e-136">Type</span></span> | <span data-ttu-id="b3c5e-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3c5e-137">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b3c5e-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3c5e-138">Authorization</span></span> | <span data-ttu-id="b3c5e-139">string</span><span class="sxs-lookup"><span data-stu-id="b3c5e-139">string</span></span> | <span data-ttu-id="b3c5e-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3c5e-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3c5e-142">Request body</span></span>

<span data-ttu-id="b3c5e-143">Nenhum corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-143">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="b3c5e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3c5e-144">Response</span></span>

<span data-ttu-id="b3c5e-145">Se tiver êxito, este método retornará o `200 OK` código de resposta com atividades do usuário para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-145">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="b3c5e-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b3c5e-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3c5e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3c5e-147">Request</span></span>

<span data-ttu-id="b3c5e-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="b3c5e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3c5e-149">Response</span></span>

<span data-ttu-id="b3c5e-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3c5e-150">The following is an example of the response.</span></span>

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
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
