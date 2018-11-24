# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="73bad-101">Obter multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="73bad-101">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="73bad-102">Obtenha uma instância do recurso que contém uma propriedade estendida com vários valores usando `$expand`.</span><span class="sxs-lookup"><span data-stu-id="73bad-102">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="73bad-103">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada.</span><span class="sxs-lookup"><span data-stu-id="73bad-103">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="73bad-104">Atualmente, esta é a única maneira de obter o objeto [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="73bad-104">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="73bad-105">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="73bad-105">The following user resources are supported:</span></span>

- [<span data-ttu-id="73bad-106">calendar</span><span class="sxs-lookup"><span data-stu-id="73bad-106">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="73bad-107">contact</span><span class="sxs-lookup"><span data-stu-id="73bad-107">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="73bad-108">contactFolder</span><span class="sxs-lookup"><span data-stu-id="73bad-108">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="73bad-109">evento</span><span class="sxs-lookup"><span data-stu-id="73bad-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="73bad-110">mailFolder</span><span class="sxs-lookup"><span data-stu-id="73bad-110">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="73bad-111">message</span><span class="sxs-lookup"><span data-stu-id="73bad-111">message</span></span>](../resources/message.md) 

<span data-ttu-id="73bad-112">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="73bad-112">As well as the following group resources:</span></span>

- <span data-ttu-id="73bad-113">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="73bad-113">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="73bad-114">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="73bad-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="73bad-115">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="73bad-115">group [post](../resources/post.md)</span></span>

<span data-ttu-id="73bad-116">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="73bad-116">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="73bad-117">Permissões</span><span class="sxs-lookup"><span data-stu-id="73bad-117">Permissions</span></span>
<span data-ttu-id="73bad-118">Dependendo do recurso estiver recebendo a propriedade estendida da e a permissão digite (delegada ou aplicativos) você solicitação, a permissão especificada na tabela a seguir é o mínimo necessário para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="73bad-118">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="73bad-119">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="73bad-119">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="73bad-120">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="73bad-120">Supported resource</span></span> | <span data-ttu-id="73bad-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73bad-121">Delegated (work or school account)</span></span> | <span data-ttu-id="73bad-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73bad-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73bad-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73bad-123">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="73bad-124">calendar</span><span class="sxs-lookup"><span data-stu-id="73bad-124">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="73bad-125">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-125">Calendars.Read</span></span> | <span data-ttu-id="73bad-126">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-126">Calendars.Read</span></span> | <span data-ttu-id="73bad-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-127">Calendars.Read</span></span> |
| [<span data-ttu-id="73bad-128">contato</span><span class="sxs-lookup"><span data-stu-id="73bad-128">contact</span></span>](../resources/contact.md) | <span data-ttu-id="73bad-129">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-129">Contacts.Read</span></span> | <span data-ttu-id="73bad-130">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-130">Contacts.Read</span></span> | <span data-ttu-id="73bad-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-131">Contacts.Read</span></span> |
| [<span data-ttu-id="73bad-132">contactFolder</span><span class="sxs-lookup"><span data-stu-id="73bad-132">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="73bad-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-133">Contacts.Read</span></span> | <span data-ttu-id="73bad-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-134">Contacts.Read</span></span> | <span data-ttu-id="73bad-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-135">Contacts.Read</span></span> |
| [<span data-ttu-id="73bad-136">evento</span><span class="sxs-lookup"><span data-stu-id="73bad-136">event</span></span>](../resources/event.md) | <span data-ttu-id="73bad-137">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-137">Calendars.Read</span></span> | <span data-ttu-id="73bad-138">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-138">Calendars.Read</span></span> |  <span data-ttu-id="73bad-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-139">Calendars.Read</span></span>|
| <span data-ttu-id="73bad-140">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="73bad-140">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="73bad-141">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bad-141">Group.Read.All</span></span> | <span data-ttu-id="73bad-142">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73bad-142">Not supported</span></span> | <span data-ttu-id="73bad-143">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73bad-143">Not supported</span></span> |
| <span data-ttu-id="73bad-144">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="73bad-144">group [event](../resources/event.md)</span></span> | <span data-ttu-id="73bad-145">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bad-145">Group.Read.All</span></span> | <span data-ttu-id="73bad-146">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73bad-146">Not supported</span></span> | <span data-ttu-id="73bad-147">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73bad-147">Not supported</span></span> |
| <span data-ttu-id="73bad-148">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="73bad-148">group [post](../resources/post.md)</span></span> | <span data-ttu-id="73bad-149">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bad-149">Group.Read.All</span></span> | <span data-ttu-id="73bad-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="73bad-150">Not supported</span></span> | <span data-ttu-id="73bad-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bad-151">Group.Read.All</span></span> |
| [<span data-ttu-id="73bad-152">mailFolder</span><span class="sxs-lookup"><span data-stu-id="73bad-152">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="73bad-153">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-153">Mail.Read</span></span> | <span data-ttu-id="73bad-154">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-154">Mail.Read</span></span> | <span data-ttu-id="73bad-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-155">Mail.Read</span></span> |
| [<span data-ttu-id="73bad-156">message</span><span class="sxs-lookup"><span data-stu-id="73bad-156">message</span></span>](../resources/message.md) | <span data-ttu-id="73bad-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-157">Mail.Read</span></span> | <span data-ttu-id="73bad-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-158">Mail.Read</span></span> | <span data-ttu-id="73bad-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="73bad-159">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="73bad-160">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73bad-160">HTTP request</span></span>

<span data-ttu-id="73bad-p103">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="73bad-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="73bad-163">Obtenha uma instância de **mensagem** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-163">Get a **message** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="73bad-164">Obtenha uma instância de **mailFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-164">Get a **mailFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="73bad-165">Obtenha uma instância do **evento** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-165">Get an **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="73bad-166">Obtenha uma instância de **calendário** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-166">Get a **calendar** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="73bad-167">Obtenha uma instância de **contato** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-167">Get a **contact** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="73bad-168">Obtenha uma instância de **contactFolder** :<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-168">Get a **contactFolder** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="73bad-169">Obtenha uma instância de **evento** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-169">Get a group **event** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="73bad-170">Obtenha uma instância de **postagem** de grupo:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="73bad-170">Get a group **post** instance: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="73bad-171">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="73bad-171">Path parameters</span></span>
|<span data-ttu-id="73bad-172">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="73bad-172">Parameter</span></span>|<span data-ttu-id="73bad-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="73bad-173">Type</span></span>|<span data-ttu-id="73bad-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bad-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73bad-175">id_value</span><span class="sxs-lookup"><span data-stu-id="73bad-175">id_value</span></span>|<span data-ttu-id="73bad-176">String</span><span class="sxs-lookup"><span data-stu-id="73bad-176">String</span></span>|<span data-ttu-id="73bad-p104">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73bad-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="73bad-181">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73bad-181">Request headers</span></span>
| <span data-ttu-id="73bad-182">Nome</span><span class="sxs-lookup"><span data-stu-id="73bad-182">Name</span></span>      |<span data-ttu-id="73bad-183">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bad-183">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73bad-184">Autorização</span><span class="sxs-lookup"><span data-stu-id="73bad-184">Authorization</span></span>  | <span data-ttu-id="73bad-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73bad-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73bad-187">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73bad-187">Request body</span></span>
<span data-ttu-id="73bad-188">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73bad-188">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73bad-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="73bad-189">Response</span></span>

<span data-ttu-id="73bad-190">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="73bad-190">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="73bad-191">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="73bad-191">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="73bad-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73bad-192">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73bad-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73bad-193">Request</span></span>
<span data-ttu-id="73bad-p106">Este exemplo obtém e expande o evento especificado incluindo uma propriedade estendida de vários valores. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="73bad-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="73bad-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="73bad-196">Response</span></span>

<span data-ttu-id="73bad-197">O corpo da resposta inclui todas as propriedades do evento especificado e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="73bad-197">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="73bad-p107">Observação: O objeto **event** mostrado aqui é truncado para concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73bad-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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