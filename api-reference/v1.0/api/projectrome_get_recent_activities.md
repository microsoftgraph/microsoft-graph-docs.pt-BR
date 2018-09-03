# <a name="get-recent-user-activities"></a><span data-ttu-id="b5145-101">Obter atividades recentes do usuário</span><span class="sxs-lookup"><span data-stu-id="b5145-101">Get recent activities</span></span>

<span data-ttu-id="b5145-102">Obter as atividades recentes de um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="b5145-102">Get recent activities for a given user.</span></span> <span data-ttu-id="b5145-103">Esta função OData tem alguns comportamentos padrão incluídos para fazê-la operar como uma API "usada mais recentemente".</span><span class="sxs-lookup"><span data-stu-id="b5145-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="b5145-104">O serviço consultará o [historyItems](../resources/projectrome_historyitem.md) mais recente e, em seguida, buscar essas atividades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="b5145-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="b5145-105">As atividades serão classificadas de acordo com o **lastModified** mais recente do **historyItem**.</span><span class="sxs-lookup"><span data-stu-id="b5145-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="b5145-106">Isso significa que atividades sem **historyItems** não serão incluídas na resposta.</span><span class="sxs-lookup"><span data-stu-id="b5145-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="b5145-107">A permissão UserActivity.ReadWrite.CreatedByApp aplicará um filtro extra à resposta para que apenas as atividades criadas pelo seu aplicativo sejam retornadas.</span><span class="sxs-lookup"><span data-stu-id="b5145-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="b5145-108">A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é especialmente ativo e se outros aplicativos criaram atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="b5145-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="b5145-109">Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="b5145-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5145-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5145-110">Permissions</span></span>

<span data-ttu-id="b5145-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b5145-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b5145-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5145-113">Permission type</span></span>      | <span data-ttu-id="b5145-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5145-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5145-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5145-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b5145-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b5145-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b5145-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5145-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5145-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="b5145-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="b5145-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5145-119">Application</span></span> | <span data-ttu-id="b5145-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5145-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5145-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5145-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5145-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5145-122">Optional query parameters</span></span>

<span data-ttu-id="b5145-123">Este método oferece suporte a alguns [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5145-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="b5145-124">São suportados os parâmetros de consulta a seguir:</span><span class="sxs-lookup"><span data-stu-id="b5145-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="b5145-125">$expand para a propriedade de navegação **historyItems**.</span><span class="sxs-lookup"><span data-stu-id="b5145-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="b5145-126">$top para limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="b5145-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="b5145-127">$filter na propriedade **lastModifiedDateTime** para **activities** ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="b5145-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="b5145-128">A seguir alguns exemplos de consultas compatíveis com a codificação de URL.</span><span class="sxs-lookup"><span data-stu-id="b5145-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="b5145-129">Cabeçalhos da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5145-129">Request headers</span></span>

|<span data-ttu-id="b5145-130">Nome</span><span class="sxs-lookup"><span data-stu-id="b5145-130">Name</span></span> | <span data-ttu-id="b5145-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5145-131">Type</span></span> | <span data-ttu-id="b5145-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5145-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="b5145-133">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5145-133">Authorization</span></span> | <span data-ttu-id="b5145-134">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5145-134">string</span></span> | <span data-ttu-id="b5145-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5145-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5145-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5145-137">Request body</span></span>

<span data-ttu-id="b5145-138">Não especifique o corpo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5145-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5145-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5145-139">Response</span></span>

<span data-ttu-id="b5145-140">Se tiver êxito, este método retornará o código de resposta`200 OK` com as atividades recentes do usuário no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b5145-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="b5145-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5145-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b5145-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5145-142">Request</span></span>

<span data-ttu-id="b5145-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5145-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="b5145-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5145-144">Response</span></span>

<span data-ttu-id="b5145-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5145-145">The following is an example of the response.</span></span>

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
              "iconUrl": "http://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "http://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "http://www.contoso.com/article?id=12345",
        "contentUrl": "http://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "http://schema.org",
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
      Property 'contentInfo' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
