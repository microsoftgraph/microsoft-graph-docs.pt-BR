# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="066ed-101">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="066ed-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="066ed-102">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="066ed-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="066ed-103">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada.</span><span class="sxs-lookup"><span data-stu-id="066ed-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the singleValueLegacyExtendedProperty object that represents an extended property.</span></span> <span data-ttu-id="066ed-104">Atualmente, esta é a única maneira de obter o objeto [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="066ed-104">Using the query parameter  allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="066ed-105">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="066ed-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="066ed-106">message</span><span class="sxs-lookup"><span data-stu-id="066ed-106">message</span></span>](../resources/message.md)
- [<span data-ttu-id="066ed-107">mailFolder</span><span class="sxs-lookup"><span data-stu-id="066ed-107">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="066ed-108">event</span><span class="sxs-lookup"><span data-stu-id="066ed-108">event</span></span>](../resources/event.md)
- [<span data-ttu-id="066ed-109">calendar</span><span class="sxs-lookup"><span data-stu-id="066ed-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="066ed-110">contact</span><span class="sxs-lookup"><span data-stu-id="066ed-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="066ed-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="066ed-111">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="066ed-112">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="066ed-112">As well as the following group resources:</span></span>

- <span data-ttu-id="066ed-113">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="066ed-113">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="066ed-114">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="066ed-114">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="066ed-115">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="066ed-115">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="066ed-116">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="066ed-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="066ed-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="066ed-117">Permissions</span></span>
<span data-ttu-id="066ed-p102">Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso que você está obtendo. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="066ed-p102">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="066ed-120">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="066ed-120">Mail.Read</span></span>
- <span data-ttu-id="066ed-121">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="066ed-121">Calendars.Read</span></span>
- <span data-ttu-id="066ed-122">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="066ed-122">Contacts.Read</span></span>
- <span data-ttu-id="066ed-123">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="066ed-123">Group.Read.All</span></span> 
 
## <a name="http-request"></a><span data-ttu-id="066ed-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="066ed-124">HTTP request</span></span>

<span data-ttu-id="066ed-p103">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL]((http://www.w3schools.com/tags/ref_urlencode.asp)) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="066ed-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding]((http://www.w3schools.com/tags/ref_urlencode.asp)) to the space characters in the filter string.</span></span>

<span data-ttu-id="066ed-127">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="066ed-127">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="066ed-128">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="066ed-128">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="066ed-129">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="066ed-129">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="066ed-130">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="066ed-130">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="066ed-131">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="066ed-131">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="066ed-132">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="066ed-132">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="066ed-133">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="066ed-133">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="066ed-134">Obtenha uma instância de **group post**:</span><span class="sxs-lookup"><span data-stu-id="066ed-134">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="parameters"></a><span data-ttu-id="066ed-135">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="066ed-135">Parameters</span></span>
|<span data-ttu-id="066ed-136">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="066ed-136">**Parameter**</span></span>|<span data-ttu-id="066ed-137">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="066ed-137">**Type**</span></span>|<span data-ttu-id="066ed-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="066ed-138">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="066ed-139">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="066ed-139">_URL parameters_</span></span>|
|<span data-ttu-id="066ed-140">id_value</span><span class="sxs-lookup"><span data-stu-id="066ed-140">id_value</span></span>|<span data-ttu-id="066ed-141">String</span><span class="sxs-lookup"><span data-stu-id="066ed-141">String</span></span>|<span data-ttu-id="066ed-p104">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="066ed-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="066ed-146">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="066ed-146">Request headers</span></span>
| <span data-ttu-id="066ed-147">Nome</span><span class="sxs-lookup"><span data-stu-id="066ed-147">Name</span></span>      |<span data-ttu-id="066ed-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="066ed-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="066ed-149">Autorização</span><span class="sxs-lookup"><span data-stu-id="066ed-149">Authorization</span></span>  | <span data-ttu-id="066ed-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="066ed-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="066ed-152">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="066ed-152">Request body</span></span>
<span data-ttu-id="066ed-153">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="066ed-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="066ed-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="066ed-154">Response</span></span>

<span data-ttu-id="066ed-155">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="066ed-155">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="066ed-156">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="066ed-156">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="066ed-157">Exemplo</span><span class="sxs-lookup"><span data-stu-id="066ed-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="066ed-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="066ed-158">Request</span></span>
<span data-ttu-id="066ed-p106">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="066ed-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="066ed-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="066ed-161">Response</span></span>

<span data-ttu-id="066ed-162">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="066ed-162">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="066ed-p107">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="066ed-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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