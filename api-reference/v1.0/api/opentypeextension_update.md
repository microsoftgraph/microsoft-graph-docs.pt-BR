# <a name="update-open-extension"></a><span data-ttu-id="599b1-101">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="599b1-101">Update open extension</span></span>

<span data-ttu-id="599b1-102">Atualize uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) com as propriedades no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="599b1-102">Update an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="599b1-103">Se uma propriedade no corpo da solicitação corresponder ao nome de uma propriedade existente na extensão, os dados na extensão serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="599b1-103">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="599b1-104">Caso contrário, essa propriedade e seus dados serão adicionados à extensão.</span><span class="sxs-lookup"><span data-stu-id="599b1-104">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="599b1-105">Os dados em uma extensão podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="599b1-105">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="599b1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="599b1-106">Permissions</span></span>

<span data-ttu-id="599b1-p101">Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso no qual a extensão foi criada. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="599b1-p101">One of the following permissions is required to call this API, depending on the resource that the extension was created in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="599b1-109">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="599b1-109">**Supported resource**</span></span>|<span data-ttu-id="599b1-110">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="599b1-110">**Permission**</span></span>|<span data-ttu-id="599b1-111">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="599b1-111">**Supported resource**</span></span>|<span data-ttu-id="599b1-112">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="599b1-112">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="599b1-113">dispositivo</span><span class="sxs-lookup"><span data-stu-id="599b1-113">device</span></span>](../resources/device.md) | <span data-ttu-id="599b1-114">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599b1-114">Device.ReadWrite.All</span></span> | [<span data-ttu-id="599b1-115">evento</span><span class="sxs-lookup"><span data-stu-id="599b1-115">event</span></span>](../resources/event.md) | <span data-ttu-id="599b1-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="599b1-116">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="599b1-117">grupo</span><span class="sxs-lookup"><span data-stu-id="599b1-117">group</span></span>](../resources/group.md) | <span data-ttu-id="599b1-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599b1-118">Group.ReadWrite.All</span></span> | [<span data-ttu-id="599b1-119">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="599b1-119">group event</span></span>](../resources/event.md) | <span data-ttu-id="599b1-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599b1-120">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="599b1-121">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="599b1-121">group post</span></span>](../resources/post.md) | <span data-ttu-id="599b1-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="599b1-122">Group.ReadWrite.All</span></span> | [<span data-ttu-id="599b1-123">mensagem</span><span class="sxs-lookup"><span data-stu-id="599b1-123">message</span></span>](../resources/message.md) | <span data-ttu-id="599b1-124">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="599b1-124">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="599b1-125">organização</span><span class="sxs-lookup"><span data-stu-id="599b1-125">organization</span></span>](../resources/organization.md) | <span data-ttu-id="599b1-126">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="599b1-126">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="599b1-127">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="599b1-127">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="599b1-128">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="599b1-128">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="599b1-129">usuário</span><span class="sxs-lookup"><span data-stu-id="599b1-129">user</span></span>](../resources/user.md) | <span data-ttu-id="599b1-130">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="599b1-130">Directory.AccessAsUser.All</span></span> | | |
 
## <a name="http-request"></a><span data-ttu-id="599b1-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="599b1-131">HTTP request</span></span>
<span data-ttu-id="599b1-132">Na solicitação, identifique a instância de recurso, use a propriedade de navegação **extensions** dessa instância para identificar a extensão e faça um `PATCH` nessa instância de extensão.</span><span class="sxs-lookup"><span data-stu-id="599b1-132">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="599b1-p102">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância do recurso, para atualizar uma extensão nele. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à atualização de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="599b1-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="599b1-135">Confira a seção [Solicitar corpo](#request-body) sobre como incluir no corpo de solicitação dados personalizados para alterar ou adicionar a essa extensão.</span><span class="sxs-lookup"><span data-stu-id="599b1-135">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>


## <a name="parameters"></a><span data-ttu-id="599b1-136">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="599b1-136">Parameters</span></span>
|<span data-ttu-id="599b1-137">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="599b1-137">**Parameter**</span></span>|<span data-ttu-id="599b1-138">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="599b1-138">**Type**</span></span>|<span data-ttu-id="599b1-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="599b1-139">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="599b1-140">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="599b1-140">_URL parameters_</span></span>|
|<span data-ttu-id="599b1-141">id</span><span class="sxs-lookup"><span data-stu-id="599b1-141">id</span></span>|<span data-ttu-id="599b1-142">string</span><span class="sxs-lookup"><span data-stu-id="599b1-142">string</span></span>|<span data-ttu-id="599b1-p103">Um identificador exclusivo para uma instância da coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="599b1-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="599b1-145">extensionId</span><span class="sxs-lookup"><span data-stu-id="599b1-145">extensionId</span></span>|<span data-ttu-id="599b1-146">string</span><span class="sxs-lookup"><span data-stu-id="599b1-146">string</span></span>|<span data-ttu-id="599b1-p104">Espaço reservado para um nome de extensão que é um identificador de texto exclusivo para a extensão ou um nome totalmente qualificado que concatena o tipo de extensão e o identificador de texto exclusivo. O nome totalmente qualificado é retornado na propriedade `id` quando você cria a extensão. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="599b1-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="599b1-150">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="599b1-150">Request headers</span></span>
| <span data-ttu-id="599b1-151">Nome</span><span class="sxs-lookup"><span data-stu-id="599b1-151">Name</span></span>       | <span data-ttu-id="599b1-152">Valor</span><span class="sxs-lookup"><span data-stu-id="599b1-152">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="599b1-153">Autorização</span><span class="sxs-lookup"><span data-stu-id="599b1-153">Authorization</span></span> | <span data-ttu-id="599b1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="599b1-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="599b1-156">Content-Type</span><span class="sxs-lookup"><span data-stu-id="599b1-156">Content-Type</span></span> | <span data-ttu-id="599b1-157">application/json</span><span class="sxs-lookup"><span data-stu-id="599b1-157">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="599b1-158">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="599b1-158">Request body</span></span>

<span data-ttu-id="599b1-p106">Forneça um corpo JSON de um objeto [openTypeExtension](../resources/openTypeExtension.md), com os seguintes pares de nome e valor obrigatórios e os dados personalizados para alterar ou adicionar a essa extensão. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="599b1-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="599b1-161">Nome</span><span class="sxs-lookup"><span data-stu-id="599b1-161">Name</span></span>       | <span data-ttu-id="599b1-162">Valor</span><span class="sxs-lookup"><span data-stu-id="599b1-162">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="599b1-163">@odata.type</span><span class="sxs-lookup"><span data-stu-id="599b1-163">@odata.type</span></span> | <span data-ttu-id="599b1-164">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="599b1-164">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="599b1-165">extensionName</span><span class="sxs-lookup"><span data-stu-id="599b1-165">extensionName</span></span> | <span data-ttu-id="599b1-166">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="599b1-166">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="599b1-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="599b1-167">Response</span></span>

<span data-ttu-id="599b1-168">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e o objeto [openTypeExtension](../resources/openTypeExtension.md) atualizado.</span><span class="sxs-lookup"><span data-stu-id="599b1-168">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/openTypeExtension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="599b1-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="599b1-169">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="599b1-170">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="599b1-170">Request 1</span></span>

<span data-ttu-id="599b1-p107">O primeiro exemplo mostra como atualizar uma extensão de uma mensagem. A extensão é representada inicialmente pela seguinte carga JSON:</span><span class="sxs-lookup"><span data-stu-id="599b1-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="599b1-173">Você pode fazer referência à extensão por seu nome:</span><span class="sxs-lookup"><span data-stu-id="599b1-173">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="599b1-174">Ou você pode fazer referência à extensão por seu nome totalmente qualificado:</span><span class="sxs-lookup"><span data-stu-id="599b1-174">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')
```

<span data-ttu-id="599b1-175">Você pode usar o exemplo de solicitação e o seguinte corpo de solicitação para atualizar a extensão acima da seguinte forma:</span><span class="sxs-lookup"><span data-stu-id="599b1-175">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="599b1-176">Alterando `companyName` de `Wingtip Toys` para `Wingtip Toys (USA)`</span><span class="sxs-lookup"><span data-stu-id="599b1-176">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="599b1-177">Alterando `dealValue` de `500050` para `500100`</span><span class="sxs-lookup"><span data-stu-id="599b1-177">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="599b1-178">Adicionar novos dados como a propriedade personalizada `updated`</span><span class="sxs-lookup"><span data-stu-id="599b1-178">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "Microsoft.Graph.OpenTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="599b1-179">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="599b1-179">Response 1</span></span>

<span data-ttu-id="599b1-180">Aqui está a resposta que é a mesma, independentemente da maneira usada para fazer referência à extensão.</span><span class="sxs-lookup"><span data-stu-id="599b1-180">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="599b1-181">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="599b1-181">Request 2</span></span>

<span data-ttu-id="599b1-p108">O segundo exemplo mostra como atualizar uma extensão em uma postagem de grupo. A extensão é representada inicialmente pela seguinte carga JSON, com um valor `expirationDate` de `2015-07-03T13:04:00Z`:</span><span class="sxs-lookup"><span data-stu-id="599b1-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="599b1-184">A seguir estão a solicitação e o corpo da solicitação para alterar o `expirationDate` para `2016-07-30T11:00:00Z`:</span><span class="sxs-lookup"><span data-stu-id="599b1-184">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
Content-type: application/json

{
   "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="599b1-185">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="599b1-185">Response 2</span></span>

<span data-ttu-id="599b1-186">Aqui está a resposta do segundo exemplo, que mostra o `expirationDate` atualizado na extensão.</span><span class="sxs-lookup"><span data-stu-id="599b1-186">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.opentypeextension"  
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
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
} -->
