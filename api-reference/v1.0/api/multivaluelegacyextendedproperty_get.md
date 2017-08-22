# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="72026-101">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="72026-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="72026-102">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="72026-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="72026-p101">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada. Atualmente, esta é a única maneira de obter o objeto [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="72026-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="72026-105">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="72026-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="72026-106">message</span><span class="sxs-lookup"><span data-stu-id="72026-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="72026-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="72026-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="72026-108">event</span><span class="sxs-lookup"><span data-stu-id="72026-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="72026-109">calendar</span><span class="sxs-lookup"><span data-stu-id="72026-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="72026-110">contact</span><span class="sxs-lookup"><span data-stu-id="72026-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="72026-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="72026-111">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="72026-112">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="72026-112">As well as the following group resources:</span></span>

- <span data-ttu-id="72026-113">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="72026-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="72026-114">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="72026-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="72026-115">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="72026-115">Group post</span></span> 

<span data-ttu-id="72026-116">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="72026-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72026-117">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72026-117">Prerequisites</span></span>
<span data-ttu-id="72026-118">Um dos seguintes valores de **scopes** é obrigatório para executar essa API, dependendo do recurso que você está obtendo:</span><span class="sxs-lookup"><span data-stu-id="72026-118">One of the following **scopes** is required to execute this API, depending on the resource you're getting:</span></span>

- <span data-ttu-id="72026-119">_Mail.Read_</span><span class="sxs-lookup"><span data-stu-id="72026-119">_Mail.Read_</span></span>
- <span data-ttu-id="72026-120">_Calendars.Read_</span><span class="sxs-lookup"><span data-stu-id="72026-120">_Calendars.Read_</span></span>
- <span data-ttu-id="72026-121">_Contacts.Read_</span><span class="sxs-lookup"><span data-stu-id="72026-121">_Contacts.Read_</span></span>
- <span data-ttu-id="72026-122">_Group.Read.All_</span><span class="sxs-lookup"><span data-stu-id="72026-122">_Group.Read.All_</span></span> 
 
## <a name="http-request"></a><span data-ttu-id="72026-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72026-123">HTTP request</span></span>

<span data-ttu-id="72026-p102">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](http://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="72026-p102">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="72026-126">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="72026-126">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72026-127">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="72026-127">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="72026-128">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="72026-128">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72026-129">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="72026-129">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72026-130">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="72026-130">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72026-131">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="72026-131">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72026-132">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="72026-132">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="72026-133">Obtenha uma instância de **group post**:</span><span class="sxs-lookup"><span data-stu-id="72026-133">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="parameters"></a><span data-ttu-id="72026-134">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="72026-134">Parameters</span></span>
|<span data-ttu-id="72026-135">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="72026-135">**Parameter**</span></span>|<span data-ttu-id="72026-136">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="72026-136">**Type**</span></span>|<span data-ttu-id="72026-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72026-137">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="72026-138">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="72026-138">_URL parameters_</span></span>|
|<span data-ttu-id="72026-139">id_value</span><span class="sxs-lookup"><span data-stu-id="72026-139">id_value</span></span>|<span data-ttu-id="72026-140">String</span><span class="sxs-lookup"><span data-stu-id="72026-140">String</span></span>|<span data-ttu-id="72026-p103">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72026-p103">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="72026-145">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72026-145">Request headers</span></span>
| <span data-ttu-id="72026-146">Nome</span><span class="sxs-lookup"><span data-stu-id="72026-146">Name</span></span>      |<span data-ttu-id="72026-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="72026-147">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72026-148">Autorização</span><span class="sxs-lookup"><span data-stu-id="72026-148">Authorization</span></span>  | <span data-ttu-id="72026-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72026-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="72026-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72026-151">Request body</span></span>
<span data-ttu-id="72026-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72026-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72026-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="72026-153">Response</span></span>

<span data-ttu-id="72026-154">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="72026-154">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="72026-155">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="72026-155">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="72026-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72026-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72026-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72026-157">Request</span></span>
<span data-ttu-id="72026-p105">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="72026-p105">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="72026-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="72026-160">Response</span></span>

<span data-ttu-id="72026-161">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="72026-161">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="72026-p106">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72026-p106">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->