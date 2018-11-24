# <a name="get-open-extension"></a><span data-ttu-id="7aece-101">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="7aece-101">Get open extension</span></span>

<span data-ttu-id="7aece-102">Obtenha uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) identificada por nome ou nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="7aece-102">Get an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) identified by name or fully qualified name.</span></span>

<span data-ttu-id="7aece-103">A tabela a seguir lista os três cenários em que é possível obter uma extensão aberta de uma instância de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="7aece-103">The following table lists the three scenarios where you can get an open extension from a supported resource instance.</span></span>

|<span data-ttu-id="7aece-104">**Cenário GET**</span><span class="sxs-lookup"><span data-stu-id="7aece-104">**GET scenario**</span></span>|<span data-ttu-id="7aece-105">**Recursos com suporte**</span><span class="sxs-lookup"><span data-stu-id="7aece-105">**Supported resources**</span></span>|<span data-ttu-id="7aece-106">**Corpo da resposta**</span><span class="sxs-lookup"><span data-stu-id="7aece-106">**Response body**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7aece-107">Obtenha uma extensão específica de uma instância de recurso conhecida.</span><span class="sxs-lookup"><span data-stu-id="7aece-107">Get a specific extension from a known resource instance.</span></span>| <span data-ttu-id="7aece-108">[Dispositivo](../resources/device.md), [evento](../resources/event.md), [grupo](../resources/group.md), [evento de grupo](../resources/event.md), [postagem de grupo](../resources/post.md), [mensagem](../resources/message.md), [organização](../resources/organization.md), [contato pessoal](../resources/contact.md), [usuário](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="7aece-108">[Device](../resources/device.md), [event](../resources/event.md), [group](../resources/group.md), [group event](../resources/event.md), [group post](../resources/post.md), [message](../resources/message.md), [organization](../resources/organization.md), [personal contact](../resources/contact.md), [user](../resources/user.md)</span></span> | <span data-ttu-id="7aece-109">Somente extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="7aece-109">Open extension only.</span></span>|
|<span data-ttu-id="7aece-110">Obtenha uma instância de recurso conhecida, expandida com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="7aece-110">Get a known resource instance expanded with a specific extension.</span></span>|<span data-ttu-id="7aece-111">Dispositivo, evento, grupo, evento de grupo, postagem de grupo, mensagem, organização, contato pessoal, usuário</span><span class="sxs-lookup"><span data-stu-id="7aece-111">Device, event, group, group event, group post, message, organization, personal contact, user</span></span> |<span data-ttu-id="7aece-112">Uma instância de recurso expandida com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="7aece-112">A resource instance expanded with the open extension.</span></span>|
|<span data-ttu-id="7aece-113">Encontre e expanda instâncias de recursos com uma extensão específica.</span><span class="sxs-lookup"><span data-stu-id="7aece-113">Find and expand resource instances with a specific extension.</span></span> |<span data-ttu-id="7aece-114">Evento, evento de grupo, postagem de grupo, mensagem, contato pessoal</span><span class="sxs-lookup"><span data-stu-id="7aece-114">Event, group event, group post, message, personal contact</span></span>|<span data-ttu-id="7aece-115">Instâncias de recursos expandidas com a extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="7aece-115">Resource instances expanded with the open extension.</span></span>|

## <a name="permissions"></a><span data-ttu-id="7aece-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="7aece-116">Permissions</span></span>

<span data-ttu-id="7aece-117">Dependendo do recurso que contém a extensão e a permissão tipo (delegado ou aplicativo) solicitada, a permissão especificada na tabela a seguir é o menos privilegiada necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="7aece-117">Depending on the resource that contains the extension and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="7aece-118">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7aece-118">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="7aece-119">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-119">Supported resource</span></span> | <span data-ttu-id="7aece-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aece-120">Delegated (work or school account)</span></span> | <span data-ttu-id="7aece-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aece-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aece-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aece-122">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="7aece-123">device</span><span class="sxs-lookup"><span data-stu-id="7aece-123">device</span></span>](../resources/device.md) | <span data-ttu-id="7aece-124">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-124">Directory.Read.All</span></span> | <span data-ttu-id="7aece-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-125">Not supported</span></span> | <span data-ttu-id="7aece-126">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aece-126">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="7aece-127">evento</span><span class="sxs-lookup"><span data-stu-id="7aece-127">event</span></span>](../resources/event.md) | <span data-ttu-id="7aece-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-128">Calendars.Read</span></span> | <span data-ttu-id="7aece-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-129">Calendars.Read</span></span> | <span data-ttu-id="7aece-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-130">Calendars.Read</span></span> |
| [<span data-ttu-id="7aece-131">group</span><span class="sxs-lookup"><span data-stu-id="7aece-131">group</span></span>](../resources/group.md) | <span data-ttu-id="7aece-132">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-132">Group.Read.All</span></span> | <span data-ttu-id="7aece-133">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-133">Not supported</span></span> | <span data-ttu-id="7aece-134">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-134">Group.Read.All</span></span> |
| [<span data-ttu-id="7aece-135">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="7aece-135">group event</span></span>](../resources/event.md) | <span data-ttu-id="7aece-136">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-136">Group.Read.All</span></span> | <span data-ttu-id="7aece-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-137">Not supported</span></span> | <span data-ttu-id="7aece-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-138">Not supported</span></span> |
| [<span data-ttu-id="7aece-139">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="7aece-139">group post</span></span>](../resources/post.md) | <span data-ttu-id="7aece-140">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-140">Group.Read.All</span></span> | <span data-ttu-id="7aece-141">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-141">Not supported</span></span> | <span data-ttu-id="7aece-142">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-142">Group.Read.All</span></span> |
| [<span data-ttu-id="7aece-143">message</span><span class="sxs-lookup"><span data-stu-id="7aece-143">message</span></span>](../resources/message.md) | <span data-ttu-id="7aece-144">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-144">Mail.Read</span></span> | <span data-ttu-id="7aece-145">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-145">Mail.Read</span></span> | <span data-ttu-id="7aece-146">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-146">Mail.Read</span></span> | 
| [<span data-ttu-id="7aece-147">organization</span><span class="sxs-lookup"><span data-stu-id="7aece-147">organization</span></span>](../resources/organization.md) | <span data-ttu-id="7aece-148">User.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-148">User.Read</span></span> | <span data-ttu-id="7aece-149">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-149">Not supported</span></span> | <span data-ttu-id="7aece-150">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7aece-150">Not supported</span></span> |
| [<span data-ttu-id="7aece-151">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="7aece-151">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="7aece-152">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-152">Contacts.Read</span></span> | <span data-ttu-id="7aece-153">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-153">Contacts.Read</span></span> | <span data-ttu-id="7aece-154">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-154">Contacts.Read</span></span> |
| [<span data-ttu-id="7aece-155">user</span><span class="sxs-lookup"><span data-stu-id="7aece-155">user</span></span>](../resources/user.md) | <span data-ttu-id="7aece-156">User.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-156">User.Read</span></span> | <span data-ttu-id="7aece-157">User.Read</span><span class="sxs-lookup"><span data-stu-id="7aece-157">User.Read</span></span> | <span data-ttu-id="7aece-158">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="7aece-158">User.Read.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="7aece-159">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aece-159">HTTP request</span></span>

<span data-ttu-id="7aece-160">Esta seção lista a sintaxe de cada um dos três cenários `GET` descritos acima</span><span class="sxs-lookup"><span data-stu-id="7aece-160">This section lists the syntax for each of the three `GET` scenarios described above.</span></span>

### <a name="get-a-specific-extension-in-a-known-resource-instance"></a><span data-ttu-id="7aece-161">Obtenha uma extensão específica em uma instância de recurso conhecida</span><span class="sxs-lookup"><span data-stu-id="7aece-161">Get a specific extension in a known resource instance</span></span>

<span data-ttu-id="7aece-162">Use a mesma solicitação REST obtendo a instância do recurso e identifique a extensão usando a propriedade de navegação **extensions** dessa instância.</span><span class="sxs-lookup"><span data-stu-id="7aece-162">Use the same REST request as getting the resource instance, and identify the extension using the **extensions** navigation property of that instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/extensions/{extensionId}
GET /groups/{Id}/events/{Id}/extensions/{extensionId}
GET /groups/{Id}/threads/{Id}/posts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/messages/{Id}/extensions/{extensionId}
GET /organization/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/contacts/{Id}/extensions/{extensionId}
GET /users/{Id|userPrincipalName}/extensions/{extensionId}
```


### <a name="get-a-known-resource-instance-expanded-with-a-matching-extension"></a><span data-ttu-id="7aece-163">Obtenha uma instância de recurso conhecida, expandida com uma extensão correspondente.</span><span class="sxs-lookup"><span data-stu-id="7aece-163">Get a known resource instance expanded with a matching extension</span></span> 

<span data-ttu-id="7aece-p102">Para os tipos de recurso de evento, evento de grupo, postagem de grupo, mensagem e contato pessoal, você pode usar a mesma solicitação REST e, enquanto obtém a instância de recurso, procure uma extensão que corresponda a um filtro em sua propriedade **id** e expanda a instância com a extensão. A resposta inclui a maioria das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="7aece-p102">For the event, group event, group post, message, personal contact resource types, you can use the same REST request as getting the resource instance, look for an extension that matches a filter on its **id** property, and expand the instance with the extension. The response includes most of the resource properties.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages/{Id}?$expand=extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts/{Id}?$expand=extensions($filter=id eq '{extensionId}')
```


<span data-ttu-id="7aece-166">Para os tipos de recurso de dispositivo, grupo, organização e usuário, você também deve usar um parâmetro `$select` para incluir a propriedade **id** e quaisquer outras propriedades que você deseja na instância do recurso:</span><span class="sxs-lookup"><span data-stu-id="7aece-166">For the device, group, organization, and user resource types, you must also use a `$select` parameter to include the **id** property and any other properties you want from the resource instance:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /groups/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /organization/{Id}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
GET /users/{Id|userPrincipalName}?$expand=extensions($filter=id eq '{extensionId}')&$select=id,{property_1},{property_n}
```

### <a name="filter-for-resource-instances-expanded-with-a-matching-extension"></a><span data-ttu-id="7aece-167">Filtrar as instâncias do recurso expandidas com uma extensão correspondente</span><span class="sxs-lookup"><span data-stu-id="7aece-167">Filter for resource instances expanded with a matching extension</span></span> 

<span data-ttu-id="7aece-168">Use a mesma solicitação REST para obter uma coleção do recurso suportado, filtre a coleção para instâncias que contêm uma extensão com uma propriedade **id** correspondente e expanda essas instâncias com a extensão.</span><span class="sxs-lookup"><span data-stu-id="7aece-168">Use the same REST request as getting a collection of the supported resource, filter the collection for instances that contain an extension with a matching **id** property, and expand these instances with the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Id|userPrincipalName}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/events?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /groups/{Id}/threads/{Id}/posts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/messages?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
GET /users/{Id|userPrincipalName}/contacts?$filter=Extensions/any(f:f/id eq '{extensionId}')&$expand=Extensions($filter=id eq '{extensionId}')
```

><span data-ttu-id="7aece-p103">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância de recurso ou coleção, para obter uma extensão dela. Todas as outras sintaxes que permitem identificar essas instâncias de recursos ou coleções dão suporte à obtenção de extensões abertas delas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="7aece-p103">**Note:** The above syntax shows some common ways to identify a resource instance or collection, in order to get an extension from it. All other syntax that allows you to identify these resource instances or collections supports getting open extensions from them in a similar way.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="7aece-171">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="7aece-171">Path parameters</span></span>
|<span data-ttu-id="7aece-172">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="7aece-172">Parameter</span></span>|<span data-ttu-id="7aece-173">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aece-173">Type</span></span>|<span data-ttu-id="7aece-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aece-174">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7aece-175">Id</span><span class="sxs-lookup"><span data-stu-id="7aece-175">Id</span></span>|<span data-ttu-id="7aece-176">string</span><span class="sxs-lookup"><span data-stu-id="7aece-176">string</span></span>|<span data-ttu-id="7aece-p104">Espaço reservado para um identificador exclusivo de um objeto na coleção correspondente, como mensagens, contatos e eventos. Obrigatório. Não deve ser confundido com a propriedade **id** de uma **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="7aece-p104">Placeholder for a unique identifier for an object in the corresponding collection such as messages, events, contacts. Required. Not to be confused with the **id** property of an **openTypeExtension**.</span></span>|
|<span data-ttu-id="7aece-180">extensionId</span><span class="sxs-lookup"><span data-stu-id="7aece-180">extensionId</span></span>|<span data-ttu-id="7aece-181">string</span><span class="sxs-lookup"><span data-stu-id="7aece-181">string</span></span>|<span data-ttu-id="7aece-p105">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para um a uma extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade **id** quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aece-p105">Placeholder for an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the **id** property when you create the extension. Required.</span></span>|

## <a name="optional-query-parameters"></a><span data-ttu-id="7aece-185">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7aece-185">Optional query parameters</span></span>

<span data-ttu-id="7aece-186">Certifique-se de aplicar a [codificação de URL](https://www.w3schools.com/tags/ref_urlencode.asp) aos caracteres de espaço na cadeia de caracteres `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7aece-186">Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the `$filter` string.</span></span>

|<span data-ttu-id="7aece-187">Nome</span><span class="sxs-lookup"><span data-stu-id="7aece-187">Name</span></span>|<span data-ttu-id="7aece-188">Valor</span><span class="sxs-lookup"><span data-stu-id="7aece-188">Value</span></span>|<span data-ttu-id="7aece-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aece-189">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="7aece-190">$filter</span><span class="sxs-lookup"><span data-stu-id="7aece-190">$filter</span></span>|<span data-ttu-id="7aece-191">string</span><span class="sxs-lookup"><span data-stu-id="7aece-191">string</span></span>|<span data-ttu-id="7aece-192">Retorna uma extensão com sua **id** correspondentes ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="7aece-192">Returns an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="7aece-193">$filter com o operador **any**</span><span class="sxs-lookup"><span data-stu-id="7aece-193">$filter with **any** operator</span></span>|<span data-ttu-id="7aece-194">string</span><span class="sxs-lookup"><span data-stu-id="7aece-194">string</span></span>|<span data-ttu-id="7aece-195">Retorna instâncias de uma coleção de recursos que contêm uma extensão com sua **id** correspondente ao valor do parâmetro `extensionId`.</span><span class="sxs-lookup"><span data-stu-id="7aece-195">Returns instances of a resource collection that contain an extension with its **id** matching the `extensionId` parameter value.</span></span>|
|<span data-ttu-id="7aece-196">$expand</span><span class="sxs-lookup"><span data-stu-id="7aece-196">$expand</span></span>|<span data-ttu-id="7aece-197">string</span><span class="sxs-lookup"><span data-stu-id="7aece-197">string</span></span>|<span data-ttu-id="7aece-198">Expande uma instância de recurso para incluir uma extensão.</span><span class="sxs-lookup"><span data-stu-id="7aece-198">Expands a resource instance to include an extension.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="7aece-199">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aece-199">Request headers</span></span>
| <span data-ttu-id="7aece-200">Nome</span><span class="sxs-lookup"><span data-stu-id="7aece-200">Name</span></span>       | <span data-ttu-id="7aece-201">Valor</span><span class="sxs-lookup"><span data-stu-id="7aece-201">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="7aece-202">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aece-202">Authorization</span></span> | <span data-ttu-id="7aece-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aece-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7aece-205">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aece-205">Request body</span></span>
<span data-ttu-id="7aece-206">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7aece-206">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7aece-207">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aece-207">Response</span></span>

<span data-ttu-id="7aece-p107">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [openTypeExtension](../resources/opentypeextension.md) no corpo da resposta. Dependendo da consulta GET, o corpo da resposta exato pode ser diferente.</span><span class="sxs-lookup"><span data-stu-id="7aece-p107">If successful, this method returns a `200 OK` response code and [openTypeExtension](../resources/opentypeextension.md) object in the response body. Depending on the GET query, the exact response body differs.</span></span>
## <a name="example"></a><span data-ttu-id="7aece-210">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7aece-210">Example</span></span>

#### <a name="request-1"></a><span data-ttu-id="7aece-211">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="7aece-211">Request 1</span></span>

<span data-ttu-id="7aece-p108">O primeiro exemplo mostra 2 maneiras de referenciar uma extensão e obtém a extensão na mensagem especificada. A resposta é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="7aece-p108">The first example shows 2 ways of referencing an extension and gets the extension in the specified message. The response is the same regardless of the way used to reference the extension.</span></span>

<span data-ttu-id="7aece-214">Em primeiro lugar, por nome:</span><span class="sxs-lookup"><span data-stu-id="7aece-214">First, by its name:</span></span> 

<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Referral", "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="7aece-215">Em segundo lugar, por ID (nome totalmente qualificado):</span><span class="sxs-lookup"><span data-stu-id="7aece-215">Second, by its ID (fully qualified name):</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

#### <a name="response-1"></a><span data-ttu-id="7aece-216">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="7aece-216">Response 1</span></span>
<span data-ttu-id="7aece-217">Veja a seguir a resposta para o primeiro exemplo.</span><span class="sxs-lookup"><span data-stu-id="7aece-217">Here is the response for the first example.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

****


#### <a name="request-2"></a><span data-ttu-id="7aece-218">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="7aece-218">Request 2</span></span>

<span data-ttu-id="7aece-219">O segundo exemplo faz referência a uma extensão por nome e obtém essa extensão no evento de grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="7aece-219">The second example references an extension by its name and gets the extension in the specified group event.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["Com.Contoso.Deal", "f5480dfd-7d77-4d0b-ba2e-3391953cc74a", "AAMkADVl17IsAAA="],
  "name": "get_opentypeextension_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/
```

#### <a name="response-2"></a><span data-ttu-id="7aece-220">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="7aece-220">Response 2</span></span>

<span data-ttu-id="7aece-221">Veja a seguir a resposta do segundo exemplo.</span><span class="sxs-lookup"><span data-stu-id="7aece-221">Here is the response from the second example.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

#### <a name="request-3"></a><span data-ttu-id="7aece-222">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="7aece-222">Request 3</span></span>

<span data-ttu-id="7aece-p109">O terceiro exemplo obtém e expande a mensagem especificada, incluindo a extensão retornada de um filtro. O filtro retorna a extensão cujo **id** corresponde a um nome totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="7aece-p109">The third example gets and expands the specified message by including the extension returned from a filter. The filter returns the extension that has its **id** matching a fully qualified name.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="],
  "name": "get_opentypeextension_3"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===?$expand=extensions($filter=id%20eq%20'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```


#### <a name="response-3"></a><span data-ttu-id="7aece-225">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="7aece-225">Response 3</span></span>

<span data-ttu-id="7aece-p110">Veja a seguir a resposta do terceiro exemplo. Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aece-p110">And here is the response from the third example. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
}
```

****

#### <a name="request-4"></a><span data-ttu-id="7aece-229">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="7aece-229">Request 4</span></span>

<span data-ttu-id="7aece-230">O quarto exemplo faz referência a uma extensão por nome totalmente qualificado e obtém essa extensão na postagem de grupo especificada.</span><span class="sxs-lookup"><span data-stu-id="7aece-230">The fourth example references an extension by its fully qualified name and gets the extension in the specified group post.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_opentypeextension_4"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
```

#### <a name="response-4"></a><span data-ttu-id="7aece-231">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="7aece-231">Response 4</span></span>

<span data-ttu-id="7aece-232">Veja a seguir a resposta do quarto exemplo.</span><span class="sxs-lookup"><span data-stu-id="7aece-232">Here is the response from the fourth example.</span></span> 

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```


#### <a name="request-5"></a><span data-ttu-id="7aece-233">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="7aece-233">Request 5</span></span>

<span data-ttu-id="7aece-p111">O quinto exemplo analisa todas as mensagens na caixa de correio do usuário conectado para localizar aquelas uma contêm uma extensão correspondente a um filtro e as expande com a inclusão dessa extensão. O filtro retorna extensões cuja propriedade **id** corresponde ao nome da extensão `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="7aece-p111">The fifth example looks at all messages in the signed-in user's mailbox to find those that contain an extension matching a filter, and expands them by including the extension. The filter returns extensions that has the **id** property matching the extension name `Com.Contoso.Referral`.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_opentypeextension_5"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Extensions/any(f:f/id%20eq%20'Com.Contoso.Referral')&$expand=Extensions($filter=id%20eq%20'Com.Contoso.Referral')
```


####<a name="response-5"></a><span data-ttu-id="7aece-236">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="7aece-236">Response 5</span></span>

<span data-ttu-id="7aece-237">Nessa resposta do quinto exemplo, há apenas uma mensagem na caixa de correio do usuário que tem uma extensão cuja **id** é igual a `Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="7aece-237">In this response for the fifth example, there is only one message in the user's mailbox that has an extension with its **id** equal to `Com.Contoso.Referral`.</span></span>

<span data-ttu-id="7aece-p112">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aece-p112">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages",
  "value": [
  {

    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')",
    "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM\"",
    "id": "AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===",
    "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AABNsWMM",
    "categories": [
    ],
    "createDateTime": "2015-06-19T02:03:31Z",
    "lastModifiedDateTime": "2015-08-13T02:28:00Z",
    "subject": "Attached is the requested info",
    "bodyPreview": "See the images attached.",
    "body": {
        "contentType": "HTML",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<style type=\"text/css\" style=\"display:none;\"><!-- P {margin-top:0;margin-bottom:0;} --></style>\r\n</head>\r\n<body dir=\"ltr\">\r\n<div id=\"divtagdefaultwrapper\" style=\"font-size:12pt;color:#000000;background-color:#FFFFFF;font-family:Calibri,Arial,Helvetica,sans-serif;\">\r\n<p>See the images attached. <br>\r\n</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "importance": "Normal",
    "hasAttachments": true,
    "parentFolderId": "AQMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===QAAAA==",
    "from": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "sender": {
        "emailAddress": {
            "address": "desmond@contoso.com",
            "name": "Desmond Raley"
        }
    },
    "toRecipients": [
        {
            "emailAddress": {
                "address": "wendy@contoso.com",
                "name": "Wendy Molina"
            }
        }
    ],
    "ccRecipients": [
    ],
    "bccRecipients": [
    ],
    "replyTo": [
    ],
    "conversationId": "AAQkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===mivdTmQ=",
    "receivedDateTime": "2015-06-19T02:05:04Z",
    "sentDateTime": "2015-06-19T02:04:59Z",
    "isDeliveryReceiptRequested": false,
    "isReadReceiptRequested": false,
    "isDraft": false,
    "isRead": true,
    "webLink": "https://outlook.office.com/owa/?ItemID=AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===%2FNJTqt5NqHlVnKVBwCY4MQpaFz9SbqUDe4%2Bbs88AAAAAAEJAACY4MQpaFz9SbqUDe4%2Bbs88AAApA4JMAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
    "inferenceClassification": "Focused",
    "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('desmond40contoso.com')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions", 
    "extensions": [ 
      { 
        "@odata.type": "#microsoft.graph.openTypeExtension",
        "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
        "extensionName": "Com.Contoso.Referral",
        "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
        "companyName": "Wingtip Toys",
        "dealValue": 500050,
        "expirationDate": "2015-12-03T10:00:00Z"
      }
     ]
  }
  ]
}

```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openTypeExtension",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/opentypeextension_get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get_opentypeextension_1, get_opentypeextension_2, get_opentypeextension_3, get_opentypeextension_5
            Unmapped tables:
        Get open extension - Unknown, Permissions - AuthScopes, Path parameters - PathParameters, Optional query parameters - PathParameters, Request headers - HttpHeaders"
  ],
  "tocPath": ""
}-->
