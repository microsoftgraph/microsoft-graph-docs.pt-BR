# <a name="get-user-activities"></a><span data-ttu-id="8fa2f-101">Obter as atividades do usuário</span><span class="sxs-lookup"><span data-stu-id="8fa2f-101">Get user activities</span></span>

<span data-ttu-id="8fa2f-102">Obter as atividades para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-102">Get activities for a given user.</span></span> <span data-ttu-id="8fa2f-103">Diferentemente da **recente** função OData, as atividades sem históricos serão retornadas.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="8fa2f-104">A permissão UserActivity.ReadWrite.CreatedByApp aplicará um filtro extra à resposta, portanto apenas as atividades criadas pelo seu aplicativo são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="8fa2f-105">A filtragem do lado do servidor pode resultar em páginas vazias se o usuário é especialmente ativo e se outros aplicativos criaram atividades mais recentes.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="8fa2f-106">Para obter as atividades do seu aplicativo, use a propriedade **nextLink** para paginar.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fa2f-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8fa2f-107">Permissions</span></span>

<span data-ttu-id="8fa2f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="8fa2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8fa2f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fa2f-110">Permission type</span></span>      | <span data-ttu-id="8fa2f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fa2f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fa2f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fa2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8fa2f-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="8fa2f-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="8fa2f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fa2f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fa2f-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="8fa2f-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="8fa2f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fa2f-116">Application</span></span> | <span data-ttu-id="8fa2f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fa2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fa2f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8fa2f-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8fa2f-119">Optional query parameters</span></span>

<span data-ttu-id="8fa2f-120">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="8fa2f-121">São suportados os parâmetros de consulta a seguir:</span><span class="sxs-lookup"><span data-stu-id="8fa2f-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="8fa2f-122">$expand para a propriedade de navegação **historyItems**.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="8fa2f-123">$top para limitar o número máximo de itens nas páginas.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="8fa2f-124">$filter na propriedade **lastModifiedDateTime** para atividades ou **historyItems**, se expandida.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="8fa2f-125">Os seguintes são alguns exemplos de consultas compatíveis com a codificação URL:</span><span class="sxs-lookup"><span data-stu-id="8fa2f-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="8fa2f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fa2f-126">Request headers</span></span>

|<span data-ttu-id="8fa2f-127">Nome</span><span class="sxs-lookup"><span data-stu-id="8fa2f-127">Name</span></span> | <span data-ttu-id="8fa2f-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fa2f-128">Type</span></span> | <span data-ttu-id="8fa2f-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fa2f-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="8fa2f-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fa2f-130">Authorization</span></span> | <span data-ttu-id="8fa2f-131">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fa2f-131">string</span></span> | <span data-ttu-id="8fa2f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fa2f-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fa2f-134">Request body</span></span>

<span data-ttu-id="8fa2f-135">Sem corpo de requisição.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-135">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="8fa2f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fa2f-136">Response</span></span>

<span data-ttu-id="8fa2f-137">Se tiver êxito, este método retornará o `200 OK` código de resposta com as atividades do usuário para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="8fa2f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fa2f-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8fa2f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fa2f-139">Request</span></span>

<span data-ttu-id="8fa2f-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="8fa2f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fa2f-141">Response</span></span>

<span data-ttu-id="8fa2f-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8fa2f-142">The following is an example of the response.</span></span>

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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
