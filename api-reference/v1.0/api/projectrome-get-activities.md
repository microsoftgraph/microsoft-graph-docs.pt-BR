---
title: Obter atividades do usuário
description: Obter atividades para um determinado usuário. Diferentemente da função OData **recente** , as atividades sem históricos serão retornadas. A permissão UserActivity. ReadWrite. CreatedByApp aplicará filtragem adicional à resposta, de modo que somente as atividades criadas por seu aplicativo serão retornadas. Essa filtragem do lado do servidor pode resultar em páginas vazias se o usuário for particularmente ativo e outros aplicativos tiverem criado atividades mais recentes. Para obter as atividades do aplicativo, use a propriedade **nextLink** para paginar.
localization_priority: Normal
ms.prod: project-rome
author: ailae
doc_type: apiPageType
ms.openlocfilehash: 0b2f9d7831a01760e871298b1df8de05a5b43978
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405880"
---
# <a name="get-user-activities"></a><span data-ttu-id="cc94e-107">Obter atividades do usuário</span><span class="sxs-lookup"><span data-stu-id="cc94e-107">Get user activities</span></span>

<span data-ttu-id="cc94e-108">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc94e-108">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc94e-109">Obter atividades para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="cc94e-109">Get activities for a given user.</span></span> <span data-ttu-id="cc94e-110">Diferentemente da função OData **recente** , as atividades sem históricos serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="cc94e-110">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="cc94e-111">A permissão UserActivity. ReadWrite. CreatedByApp aplicará filtragem adicional à resposta, de modo que somente as atividades criadas por seu aplicativo serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="cc94e-111">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="cc94e-112">Essa filtragem do lado do servidor pode resultar em páginas vazias se o usuário for particularmente ativo e outros aplicativos tiverem criado atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="cc94e-112">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="cc94e-113">Para obter as atividades do aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="cc94e-113">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc94e-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="cc94e-114">Permissions</span></span>

<span data-ttu-id="cc94e-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc94e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc94e-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc94e-117">Permission type</span></span>      | <span data-ttu-id="cc94e-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cc94e-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc94e-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc94e-119">Delegated (work or school account)</span></span> | <span data-ttu-id="cc94e-120">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="cc94e-120">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="cc94e-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc94e-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc94e-122">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="cc94e-122">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="cc94e-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc94e-123">Application</span></span> | <span data-ttu-id="cc94e-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc94e-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc94e-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc94e-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc94e-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cc94e-126">Optional query parameters</span></span>

<span data-ttu-id="cc94e-127">Este método oferece suporte a alguns [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cc94e-127">This method supports some [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="cc94e-128">Há suporte para os seguintes parâmetros de consulta:</span><span class="sxs-lookup"><span data-stu-id="cc94e-128">The following query parameters are supported:</span></span>

- <span data-ttu-id="cc94e-129">$expand da propriedade de navegação **historyItems** .</span><span class="sxs-lookup"><span data-stu-id="cc94e-129">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="cc94e-130">$top limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="cc94e-130">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="cc94e-131">$filter na propriedade **lastModifiedDateTime** para atividades ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="cc94e-131">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="cc94e-132">Veja a seguir alguns exemplos de consultas suportadas com codificação de URL:</span><span class="sxs-lookup"><span data-stu-id="cc94e-132">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="cc94e-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc94e-133">Request headers</span></span>

|<span data-ttu-id="cc94e-134">Nome</span><span class="sxs-lookup"><span data-stu-id="cc94e-134">Name</span></span> | <span data-ttu-id="cc94e-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc94e-135">Type</span></span> | <span data-ttu-id="cc94e-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc94e-136">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="cc94e-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc94e-137">Authorization</span></span> | <span data-ttu-id="cc94e-138">string</span><span class="sxs-lookup"><span data-stu-id="cc94e-138">string</span></span> | <span data-ttu-id="cc94e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc94e-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc94e-141">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc94e-141">Request body</span></span>

<span data-ttu-id="cc94e-142">Nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc94e-142">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="cc94e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc94e-143">Response</span></span>

<span data-ttu-id="cc94e-144">Se bem-sucedido, este método retorna o `200 OK` código de resposta com as atividades do usuário para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc94e-144">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="cc94e-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc94e-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cc94e-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc94e-146">Request</span></span>

<span data-ttu-id="cc94e-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc94e-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="cc94e-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc94e-148">Response</span></span>

<span data-ttu-id="cc94e-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cc94e-149">The following is an example of the response.</span></span>

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