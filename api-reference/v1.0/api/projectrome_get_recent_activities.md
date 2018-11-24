# <a name="get-recent-user-activities"></a><span data-ttu-id="87788-101">Obtenha as atividades recentes do usuário</span><span class="sxs-lookup"><span data-stu-id="87788-101">Get recent user activities</span></span>

<span data-ttu-id="87788-102">Obtenha atividades recentes para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="87788-102">Get recent activities for a given user.</span></span> <span data-ttu-id="87788-103">Esta função de OData tem alguns comportamentos padrão incluídos para torná-lo a operar como uma API "usado mais recentemente".</span><span class="sxs-lookup"><span data-stu-id="87788-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="87788-104">O serviço de consulta para o mais recente [historyItems](../resources/projectrome_historyitem.md)e, em seguida, coloque essas atividades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="87788-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="87788-105">Atividades serão classificadas de acordo com o **lastModified** mais recentes sobre o **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="87788-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="87788-106">Isso significa que atividades sem **historyItems** não serão incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="87788-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="87788-107">A permissão de UserActivity.ReadWrite.CreatedByApp também se aplicará filtragem extra à resposta, para que apenas as atividades criadas pelo seu aplicativo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="87788-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="87788-108">A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é particularmente ativo e outros aplicativos criou atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="87788-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="87788-109">Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="87788-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="87788-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="87788-110">Permissions</span></span>

<span data-ttu-id="87788-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87788-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87788-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87788-113">Permission type</span></span>      | <span data-ttu-id="87788-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87788-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87788-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87788-115">Delegated (work or school account)</span></span> | <span data-ttu-id="87788-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="87788-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="87788-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87788-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87788-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="87788-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="87788-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87788-119">Application</span></span> | <span data-ttu-id="87788-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87788-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87788-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87788-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87788-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87788-122">Optional query parameters</span></span>

<span data-ttu-id="87788-123">Este método oferece suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87788-123">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="87788-124">Os parâmetros de consulta a seguir são suportados:</span><span class="sxs-lookup"><span data-stu-id="87788-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="87788-125">$expand para a propriedade de navegação **historyItems** .</span><span class="sxs-lookup"><span data-stu-id="87788-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="87788-126">$top para limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="87788-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="87788-127">$filter na propriedade **lastModifiedDateTime** para **atividades** ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="87788-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="87788-128">A seguir estão alguns exemplos de consultas compatíveis com a codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="87788-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="87788-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87788-129">Request headers</span></span>

|<span data-ttu-id="87788-130">Nome</span><span class="sxs-lookup"><span data-stu-id="87788-130">Name</span></span> | <span data-ttu-id="87788-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="87788-131">Type</span></span> | <span data-ttu-id="87788-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="87788-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="87788-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="87788-133">Authorization</span></span> | <span data-ttu-id="87788-134">string</span><span class="sxs-lookup"><span data-stu-id="87788-134">string</span></span> | <span data-ttu-id="87788-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87788-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="87788-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87788-137">Request body</span></span>

<span data-ttu-id="87788-138">Não especifique o corpo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87788-138">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="87788-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="87788-139">Response</span></span>

<span data-ttu-id="87788-140">Se tiver êxito, este método retornará o `200 OK` código de resposta com a atividades recentes do usuário para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="87788-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="87788-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87788-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="87788-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87788-142">Request</span></span>

<span data-ttu-id="87788-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87788-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="87788-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="87788-144">Response</span></span>

<span data-ttu-id="87788-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87788-145">The following is an example of the response.</span></span>

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
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements:
      Schema validation failed on property 'visualElements' ['microsoft.graph.visualInfo']",

    "Warning: get_recent_activities/container/visualElements/content:
      Schema validation failed on property 'content' ['microsoft.graph.Json']",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
