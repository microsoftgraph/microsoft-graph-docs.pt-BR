# <a name="get-singlevaluelegacyextendedproperty"></a><span data-ttu-id="1baed-101">Obter singleValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="1baed-101">Get singleValueLegacyExtendedProperty</span></span>

<span data-ttu-id="1baed-102">Obtenha instâncias de recursos que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`.</span><span class="sxs-lookup"><span data-stu-id="1baed-102">Get resource instances that contain a single-value extended property by using `$expand` or `$filter`.</span></span>

<span data-ttu-id="1baed-p101">Usar o parâmetro de consulta `$expand` permite que você obtenha a instância especificada expandida com a propriedade estendida indicada. Atualmente, esta é a única maneira de obter o objeto [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) que representa uma propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1baed-p101">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property. This is currently the only way to get the [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="1baed-p102">Usar o parâmetro de consulta `$filter` permite obter todas as instâncias do recurso especificado que têm uma correspondência estendida correspondente a um filtro nas propriedades **id** e **value**. O filtro é aplicado a todas as instâncias do recurso na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="1baed-p102">Using the query parameter `$filter` allows you to get all the instances of the specified resource that have an extended property matching a filter on the **id** and **value** properties. The filter is applied to all instances of the resource in the signed-in user's mailbox.</span></span>

<span data-ttu-id="1baed-107">Há suporte para as seguintes fontes de dados:</span><span class="sxs-lookup"><span data-stu-id="1baed-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="1baed-108">message</span><span class="sxs-lookup"><span data-stu-id="1baed-108">message</span></span>](../resources/message.md)
- [<span data-ttu-id="1baed-109">mailFolder</span><span class="sxs-lookup"><span data-stu-id="1baed-109">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="1baed-110">event</span><span class="sxs-lookup"><span data-stu-id="1baed-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="1baed-111">calendar</span><span class="sxs-lookup"><span data-stu-id="1baed-111">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="1baed-112">contact</span><span class="sxs-lookup"><span data-stu-id="1baed-112">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="1baed-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="1baed-113">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="1baed-114">Também há suporte para os seguintes recursos de grupo:</span><span class="sxs-lookup"><span data-stu-id="1baed-114">As well as the following group resources:</span></span>

- <span data-ttu-id="1baed-115">grupo [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="1baed-115">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="1baed-116">grupo [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="1baed-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="1baed-117">grupo [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="1baed-117">group [post](../resources/post.md)</span></span> 

<span data-ttu-id="1baed-118">Confira [Visão geral de propriedades estendidas](../resources/extended-properties-overview.md) para saber mais sobre quando usar extensões abertas ou propriedades estendidas e sobre como especificar propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="1baed-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1baed-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="1baed-119">Permissions</span></span>
<span data-ttu-id="1baed-p103">Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso que você está obtendo. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1baed-p103">One of the following permissions is required to call this API, depending on the resource you're getting. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

- <span data-ttu-id="1baed-122">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="1baed-122">Mail.Read</span></span>
- <span data-ttu-id="1baed-123">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1baed-123">Calendars.Read</span></span>
- <span data-ttu-id="1baed-124">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1baed-124">Contacts.Read</span></span>
- <span data-ttu-id="1baed-125">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="1baed-125">Group.Read.All</span></span> 

## <a name="http-request"></a><span data-ttu-id="1baed-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1baed-126">HTTP request</span></span>

#### <a name="get-a-resource-instance-using-expand"></a><span data-ttu-id="1baed-127">OBTER uma instância de recurso usando `$expand`</span><span class="sxs-lookup"><span data-stu-id="1baed-127">GET a resource instance using `$expand`</span></span>
<span data-ttu-id="1baed-p104">Obtenha uma instância de recurso expandida com uma propriedade estendida que corresponde a um filtro na propriedade **id**. Aplique a [codificação de URL](http://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de filtro.</span><span class="sxs-lookup"><span data-stu-id="1baed-p104">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="1baed-130">Obtenha uma instância de **message**:</span><span class="sxs-lookup"><span data-stu-id="1baed-130">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1baed-131">Obtenha uma instância de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="1baed-131">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1baed-132">Obtenha uma instância de **event**:</span><span class="sxs-lookup"><span data-stu-id="1baed-132">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1baed-133">Obtenha uma instância de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="1baed-133">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1baed-134">Obtenha uma instância de **contact**:</span><span class="sxs-lookup"><span data-stu-id="1baed-134">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1baed-135">Obtenha uma instância de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="1baed-135">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="1baed-136">Obtenha uma instância de **group event**:</span><span class="sxs-lookup"><span data-stu-id="1baed-136">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="1baed-137">Obtenha uma instância de **group post**:</span><span class="sxs-lookup"><span data-stu-id="1baed-137">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=singleValueExtendedProperties($filter=id eq '{id_value}')
```

#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="1baed-138">OBTER instâncias de recursos usando `$filter`</span><span class="sxs-lookup"><span data-stu-id="1baed-138">GET resource instances using `$filter`</span></span>

<span data-ttu-id="1baed-p105">Obtenha instâncias de um recurso com suporte que tenham a propriedade estendida correspondente a um filtro nas propriedades **id** e **value**. Certifique-se de aplicar a [codificação de URL](http://www.w3schools.com/tags/ref_urlencode.asp) aos seguintes caracteres na cadeia de filtro - barra e espaço.</span><span class="sxs-lookup"><span data-stu-id="1baed-p105">Get instances of a supported resource that have the extended property matching a filter on the **id** and **value** properties. Make sure you apply [URL encoding](http://www.w3schools.com/tags/ref_urlencode.asp) to the following characters in the filter string - forward slash and space.</span></span>


<span data-ttu-id="1baed-141">Obtenha instâncias de **message**:</span><span class="sxs-lookup"><span data-stu-id="1baed-141">Get **message** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/mailFolders/{id}/messages?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1baed-142">Obtenha instâncias de **mailFolder**:</span><span class="sxs-lookup"><span data-stu-id="1baed-142">Get **mailFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/mailFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="1baed-143">Obtenha instâncias de **event**:</span><span class="sxs-lookup"><span data-stu-id="1baed-143">Get **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1baed-144">Obtenha instâncias de **calendar**:</span><span class="sxs-lookup"><span data-stu-id="1baed-144">Get **calendar** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/calendars?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1baed-145">Obtenha instâncias de **contact**:</span><span class="sxs-lookup"><span data-stu-id="1baed-145">Get **contact** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /me/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1baed-146">Obtenha instâncias de **contactFolder**:</span><span class="sxs-lookup"><span data-stu-id="1baed-146">Get **contactFolder** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /users/{id|userPrincipalName}/contactFolders?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```
<span data-ttu-id="1baed-147">Obtenha instâncias de **group event**:</span><span class="sxs-lookup"><span data-stu-id="1baed-147">Get group **event** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

<span data-ttu-id="1baed-148">Obtenha instâncias de **group post**:</span><span class="sxs-lookup"><span data-stu-id="1baed-148">Get group **post** instances:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts?$filter=singleValueExtendedProperties/Any(ep: ep/id eq '{id_value}' and ep/value eq '{property_value}')
```

## <a name="parameters"></a><span data-ttu-id="1baed-149">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="1baed-149">Parameters</span></span>
|<span data-ttu-id="1baed-150">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="1baed-150">**Parameter**</span></span>|<span data-ttu-id="1baed-151">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="1baed-151">**Type**</span></span>|<span data-ttu-id="1baed-152">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1baed-152">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1baed-153">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="1baed-153">_URL parameters_</span></span>|
|<span data-ttu-id="1baed-154">id_value</span><span class="sxs-lookup"><span data-stu-id="1baed-154">id_value</span></span>|<span data-ttu-id="1baed-155">String</span><span class="sxs-lookup"><span data-stu-id="1baed-155">String</span></span>|<span data-ttu-id="1baed-p106">A ID da propriedade estendida a ser correspondida. Ele deve seguir um dos formatos com suporte. Para saber mais, confira [Visão geral das propriedades estendidas do Outlook](../resources/extended-properties-overview.md). Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1baed-p106">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|
|<span data-ttu-id="1baed-160">property_value</span><span class="sxs-lookup"><span data-stu-id="1baed-160">property_value</span></span>|<span data-ttu-id="1baed-161">String</span><span class="sxs-lookup"><span data-stu-id="1baed-161">String</span></span>|<span data-ttu-id="1baed-p107">O valor da propriedade estendida a ser correspondida. Obrigatório onde listado na seção **Solicitação HTTP** acima.</span><span class="sxs-lookup"><span data-stu-id="1baed-p107">The value of the extended property to match. Required where listed in the **HTTP request** section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="1baed-164">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1baed-164">Request headers</span></span>
| <span data-ttu-id="1baed-165">Nome</span><span class="sxs-lookup"><span data-stu-id="1baed-165">Name</span></span>      |<span data-ttu-id="1baed-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="1baed-166">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1baed-167">Autorização</span><span class="sxs-lookup"><span data-stu-id="1baed-167">Authorization</span></span>  | <span data-ttu-id="1baed-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1baed-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1baed-170">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1baed-170">Request body</span></span>
<span data-ttu-id="1baed-171">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1baed-171">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1baed-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="1baed-172">Response</span></span>

<span data-ttu-id="1baed-173">Se bem-sucedido, este método retorna um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="1baed-173">If successful, this method returns a `200 OK` response code.</span></span>

#### <a name="get-resource-instance-using-expand"></a><span data-ttu-id="1baed-174">OBTER instância de recurso usando `$expand`</span><span class="sxs-lookup"><span data-stu-id="1baed-174">GET resource instance using `$expand`</span></span>
<span data-ttu-id="1baed-175">O corpo da resposta inclui um objeto que representa a instância de recurso solicitada, expandida com o objeto [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) correspondente.</span><span class="sxs-lookup"><span data-stu-id="1baed-175">The response body includes an object representing the requested resource instance, expanded with the matching [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.</span></span>
  
#### <a name="get-resource-instances-using-filter"></a><span data-ttu-id="1baed-176">OBTER instâncias de recursos usando `$filter`</span><span class="sxs-lookup"><span data-stu-id="1baed-176">GET resource instances using `$filter`</span></span>
<span data-ttu-id="1baed-p109">O corpo da resposta inclui um ou mais objetos que representam as instâncias de recursos contendo a propriedade estendida correspondente. O corpo da resposta não inclui a propriedade estendida.</span><span class="sxs-lookup"><span data-stu-id="1baed-p109">The response body includes one or more objects representing the resource instances that contain the matching extended property. The response body does not include the extended property.</span></span>

## <a name="example"></a><span data-ttu-id="1baed-179">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1baed-179">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="1baed-180">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="1baed-180">Request 1</span></span>

<span data-ttu-id="1baed-p110">O primeiro exemplo obtém e expande a mensagem especificada, incluindo uma propriedade estendida de valor único. O filtro retorna a propriedade estendida cuja **id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="1baed-p110">The first example gets and expands the specified message by including a single-value extended property. The filter returns the extended property that has its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')?$expand=singleValueExtendedProperties($filter=id%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color')
```
##### <a name="response-1"></a><span data-ttu-id="1baed-183">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="1baed-183">Response 1</span></span>
<span data-ttu-id="1baed-184">O corpo da resposta inclui todas as propriedades da mensagem especificada e a propriedade estendida retornada do filtro.</span><span class="sxs-lookup"><span data-stu-id="1baed-184">The response body includes all the properties of the specified message and extended property returned from the filter.</span></span>

<span data-ttu-id="1baed-p111">Observação: O objeto **message** mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1baed-p111">Note: The **message** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/messages('AAMkAGE1M2_bs88AACHsLqWAAA=')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AACbyS4H\"",
    "id": "AAMkAGE1M2_bs88AACHsLqWAAA=",
    "subject": "RE: Talk about emergency prep",
    "sender": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "from": null,
    "toRecipients": [
        {
            "emailAddress": {
                "name": "Christine Irwin",
                "address": "christine@contoso.com"
            }
        }
    ],
    "singleValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2_bs88AACHsLqWAAA%3D')/singleValueExtendedProperties",
    "singleValueExtendedProperties": [
        {
            "id": "String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color",
            "value": "Green"
        }
    ]
}
```

****

#### <a name="request-2"></a><span data-ttu-id="1baed-187">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="1baed-187">Request 2</span></span>

<span data-ttu-id="1baed-p112">O segundo exemplo obtém mensagens que possuem a propriedade estendida de valor único especificada no filtro. O filtro retorna a propriedade estendida cujo valor de:</span><span class="sxs-lookup"><span data-stu-id="1baed-p112">The second example gets messages that have the single-value extended property specified in the filter. The filter returns the extended property that has:</span></span>
- <span data-ttu-id="1baed-190">**id** corresponde à cadeia de caracteres `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (com a URL de codificação removida aqui para facilitar a leitura).</span><span class="sxs-lookup"><span data-stu-id="1baed-190">Its **id** matching the string `String {66f5a359-4659-4830-9070-00047ec6ac6e} Name Color` (with URL encoding removed here for ease of reading).</span></span>
- <span data-ttu-id="1baed-191">**value** é igual a `Green`.</span><span class="sxs-lookup"><span data-stu-id="1baed-191">Its **value** being `Green`.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/api/v1.0/Me/messages?$filter=singleValueExtendedProperties%2FAny(ep%3A%20ep%2Fid%20eq%20'String%20{66f5a359-4659-4830-9070-00047ec6ac6e}%20Name%20Color'%20and%20ep%2Fvalue%20eq%20'Green')
```

##### <a name="response-2"></a><span data-ttu-id="1baed-192">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="1baed-192">Response 2</span></span>

<span data-ttu-id="1baed-p113">Uma resposta bem-sucedida é indicada por um código de resposta `HTTP 200 OK`, e o corpo da resposta inclui todas as propriedades das mensagens cuja propriedade estendida corresponde ao filtro. O corpo da resposta é semelhante à resposta da [obtenção de uma coleção de mensagens](../api/user_list_messages.md). A resposta não inclui a propriedade estendida correspondente.</span><span class="sxs-lookup"><span data-stu-id="1baed-p113">A successful response is indicated by an `HTTP 200 OK` response code, and the response body includes all the properties of the messages that have the extended property matching the filter. The response body is similar to the response from [getting a message collection](../api/user_list_messages.md). The response does not include the matching extended property.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get singleValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->