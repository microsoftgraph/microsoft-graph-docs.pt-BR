# <a name="create-open-extension"></a><span data-ttu-id="b543b-101">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="b543b-101">Create open extension</span></span>

<span data-ttu-id="b543b-102">Crie uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="b543b-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b543b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="b543b-103">Permissions</span></span>

<span data-ttu-id="b543b-p101">Uma das seguintes permissões é necessária para chamar essa API, dependendo do recurso no qual você está criando a extensão. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b543b-p101">One of the following permissions is required to call this API, depending on the resource you're creating the extension in. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b543b-106">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="b543b-106">**Supported resource**</span></span>|<span data-ttu-id="b543b-107">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="b543b-107">**Permission**</span></span>|<span data-ttu-id="b543b-108">**Recurso com suporte**</span><span class="sxs-lookup"><span data-stu-id="b543b-108">**Supported resource**</span></span>|<span data-ttu-id="b543b-109">**Permissão**</span><span class="sxs-lookup"><span data-stu-id="b543b-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="b543b-110">dispositivo</span><span class="sxs-lookup"><span data-stu-id="b543b-110">device</span></span>](../resources/device.md) | <span data-ttu-id="b543b-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b543b-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="b543b-112">evento</span><span class="sxs-lookup"><span data-stu-id="b543b-112">event</span></span>](../resources/event.md) | <span data-ttu-id="b543b-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b543b-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="b543b-114">grupo</span><span class="sxs-lookup"><span data-stu-id="b543b-114">group</span></span>](../resources/group.md) | <span data-ttu-id="b543b-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b543b-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="b543b-116">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="b543b-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="b543b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b543b-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="b543b-118">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="b543b-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="b543b-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b543b-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="b543b-120">mensagem</span><span class="sxs-lookup"><span data-stu-id="b543b-120">message</span></span>](../resources/message.md) | <span data-ttu-id="b543b-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b543b-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="b543b-122">organização</span><span class="sxs-lookup"><span data-stu-id="b543b-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="b543b-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b543b-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="b543b-124">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="b543b-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="b543b-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b543b-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="b543b-126">usuário</span><span class="sxs-lookup"><span data-stu-id="b543b-126">user</span></span>](../resources/user.md) | <span data-ttu-id="b543b-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b543b-127">Directory.AccessAsUser.All</span></span> | | |
 
## <a name="http-request"></a><span data-ttu-id="b543b-128">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b543b-128">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="b543b-129">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="b543b-129">Create an extension in a new resource instance</span></span>

<span data-ttu-id="b543b-130">Use a mesma solicitação REST conforme cria da instância.</span><span class="sxs-lookup"><span data-stu-id="b543b-130">Use the same REST request as creating the instance.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="b543b-p102">**Observação:** A sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte. Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="b543b-p102">**Note:** The above syntax shows some common ways to create the supported resource instances. All other POST syntax that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="b543b-133">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b543b-133">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="b543b-134">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="b543b-134">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="b543b-135">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="b543b-135">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /devices/{id}/extensions
POST /users/{id|userPrincipalName}/events/{id}/extensions
POST /groups/{id}/extensions
POST /groups/{id}/events/{id}/extensions
POST /groups/{id}/threads/{id}/posts/{id}/extensions
POST /users/{id|userPrincipalName}/messages/{id}/extensions
POST /organization/{id}/extensions
POST /users/{id|userPrincipalName}/contacts/{id}/extensions
POST /users/{id|userPrincipalName}/extensions
```

><span data-ttu-id="b543b-p103">**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância do recurso, para criar uma extensão nele. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="b543b-p103">**Note:** The above syntax shows some common ways to identify a resource instance, in order to create an extension in it. All other syntax that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="b543b-138">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b543b-138">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="parameters"></a><span data-ttu-id="b543b-139">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="b543b-139">Parameters</span></span>
|<span data-ttu-id="b543b-140">**Parâmetro**</span><span class="sxs-lookup"><span data-stu-id="b543b-140">**Parameter**</span></span>|<span data-ttu-id="b543b-141">**Tipo**</span><span class="sxs-lookup"><span data-stu-id="b543b-141">**Type**</span></span>|<span data-ttu-id="b543b-142">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b543b-142">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b543b-143">_Parâmetros de URL_</span><span class="sxs-lookup"><span data-stu-id="b543b-143">_URL parameters_</span></span>|
|<span data-ttu-id="b543b-144">id</span><span class="sxs-lookup"><span data-stu-id="b543b-144">id</span></span>|<span data-ttu-id="b543b-145">string</span><span class="sxs-lookup"><span data-stu-id="b543b-145">string</span></span>|<span data-ttu-id="b543b-p104">Um identificador exclusivo para um objeto na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b543b-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|


## <a name="request-headers"></a><span data-ttu-id="b543b-148">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b543b-148">Request headers</span></span>
| <span data-ttu-id="b543b-149">Nome</span><span class="sxs-lookup"><span data-stu-id="b543b-149">Name</span></span>       | <span data-ttu-id="b543b-150">Valor</span><span class="sxs-lookup"><span data-stu-id="b543b-150">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b543b-151">Autorização</span><span class="sxs-lookup"><span data-stu-id="b543b-151">Authorization</span></span> | <span data-ttu-id="b543b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b543b-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b543b-154">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b543b-154">Content-Type</span></span> | <span data-ttu-id="b543b-155">application/json</span><span class="sxs-lookup"><span data-stu-id="b543b-155">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b543b-156">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b543b-156">Request body</span></span>

<span data-ttu-id="b543b-p106">Forneça um corpo JSON de uma [openTypeExtension](../resources/openTypeExtension.md), com os seguintes pares de nome/valor obrigatórios e dados personalizados adicionais. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="b543b-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="b543b-159">Name</span><span class="sxs-lookup"><span data-stu-id="b543b-159">Name</span></span>       | <span data-ttu-id="b543b-160">Valor</span><span class="sxs-lookup"><span data-stu-id="b543b-160">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b543b-161">@odata.type</span><span class="sxs-lookup"><span data-stu-id="b543b-161">@odata.type</span></span> | <span data-ttu-id="b543b-162">Microsoft.Graph.OpenTypeExtension</span><span class="sxs-lookup"><span data-stu-id="b543b-162">Microsoft.Graph.OpenTypeExtension</span></span> |
| <span data-ttu-id="b543b-163">extensionName</span><span class="sxs-lookup"><span data-stu-id="b543b-163">extensionName</span></span> | <span data-ttu-id="b543b-164">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="b543b-164">%unique_string%</span></span> |

<span data-ttu-id="b543b-165">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="b543b-165">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="b543b-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b543b-166">Response</span></span>

#### <a name="response-code"></a><span data-ttu-id="b543b-167">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="b543b-167">Response code</span></span>
<span data-ttu-id="b543b-168">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="b543b-168">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="b543b-p107">Ao criar uma extensão na mesma operação como criação de uma instância de recurso, uma operação bem-sucedida retorna o mesmo código de resposta que quando a operação é usada para criar apenas a instância de recurso sem a extensão. Consulte os tópicos correspondentes para criar a instância conforme listado [cima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="b543b-p107">When creating an extension in the same operation as creating a resource instance, a successful operation returns the same response code as when the operation is used to create only the resource instance without the extension. Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

#### <a name="response-body"></a><span data-ttu-id="b543b-171">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="b543b-171">Response body</span></span>
| <span data-ttu-id="b543b-172">Cenário</span><span class="sxs-lookup"><span data-stu-id="b543b-172">Scenario</span></span>       | <span data-ttu-id="b543b-173">Recurso</span><span class="sxs-lookup"><span data-stu-id="b543b-173">Resource</span></span>  | <span data-ttu-id="b543b-174">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="b543b-174">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="b543b-175">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="b543b-175">Creating an extension while explicitly creating a _new_ resource instance</span></span> | [<span data-ttu-id="b543b-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span><span class="sxs-lookup"><span data-stu-id="b543b-176">contact](../resources/contact.md), [event](../resources/event.md), [message</span></span>](../resources/message.md) | <span data-ttu-id="b543b-177">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/openTypeExtension.md).</span><span class="sxs-lookup"><span data-stu-id="b543b-177">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="b543b-178">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="b543b-178">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="b543b-179">postagem</span><span class="sxs-lookup"><span data-stu-id="b543b-179">post</span></span>](../resources/post.md) | <span data-ttu-id="b543b-180">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b543b-180">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="b543b-181">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="b543b-181">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="b543b-182">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="b543b-182">All supported resources</span></span> | <span data-ttu-id="b543b-183">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="b543b-183">Includes the **openTypeExtension** object.</span></span> |
 


## <a name="example"></a><span data-ttu-id="b543b-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b543b-184">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b543b-185">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="b543b-185">Request 1</span></span>

<span data-ttu-id="b543b-p108">O primeiro exemplo cria uma mensagem e uma extensão na mesma chamada. O corpo da solicitação inclui o seguinte:</span><span class="sxs-lookup"><span data-stu-id="b543b-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="b543b-188">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="b543b-188">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span> 
- <span data-ttu-id="b543b-189">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-189">And for the extension:</span></span>

  - <span data-ttu-id="b543b-190">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="b543b-190">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
  - <span data-ttu-id="b543b-191">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="b543b-191">The extension name "Com.Contoso.Referral".</span></span> 
  - <span data-ttu-id="b543b-192">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="b543b-192">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages

{
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "You should be proud!"
  },
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com"
      }
    }
  ],
  "extensions": [
    {
      "@odata.type": "Microsoft.Graph.OpenTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

##### <a name="response-1"></a><span data-ttu-id="b543b-193">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="b543b-193">Response 1</span></span>

<span data-ttu-id="b543b-p109">Veja a seguir a resposta para o primeiro exemplo. O corpo da resposta inclui propriedades da nova mensagem e o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="b543b-196">A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="b543b-196">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="b543b-197">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="b543b-197">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="b543b-198">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="b543b-198">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="b543b-p110">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b543b-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages/$entity",
  "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')",
  "@odata.etag": "W/\"CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj\"",
  "id": "AAMkAGEbs88AAB84uLuAAA=",
  "createdDateTime": "2015-10-30T03:03:43Z",
  "lastModifiedDateTime": "2015-10-30T03:03:43Z",
  "changeKey": "CQAAABYAAACY4MQpaFz9SbqUDe4+bs88AAB88LOj",
  "categories": [ ],
  "receivedDateTime": "2015-10-30T03:03:43Z",
  "sentDateTime": "2015-10-30T03:03:43Z",
  "hasAttachments": false,
  "subject": "Annual review",
  "body": {
    "contentType": "HTML",
    "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r
\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nYou should be proud!\r\n</body>\r
\n</html>\r\n"
  },
  "bodyPreview": "You should be proud!",
  "importance": "Normal",
  "parentFolderId": "AQMkAGEwAAAIBDwAAAA==",
  "sender": null,
  "from": null,
  "toRecipients": [
    {
      "emailAddress": {
        "address": "rufus@contoso.com",
        "name": "John Doe"
      }
    }
  ],
  "ccRecipients": [ ],
  "bccRecipients": [ ],
  "replyTo": [ ],
  "conversationId": "AAQkAGEFGugh3SVdMzzc=",
  "isDeliveryReceiptRequested": false,
  "isReadReceiptRequested": false,
  "isRead": true,
  "isDraft": true,
  "webLink": "https://outlook.office.com/owa/?
ItemID=AAMkAGEbs88AAB84uLuAAA%3D&exvsurl=1&viewmodel=ReadMessageItem",
  "inferenceClassification": "Focused",
  "extensions@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages
('AAMkAGEbs88AAB84uLuAAA%3D')/extensions",
  "extensions": [
    {
      "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
      "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df800e5@1717f226-49d1-4d0c-9d74-709fad664b77')/messages
('AAMkAGEbs88AAB84uLuAAA=')/extensions('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
      "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```


****

##### <a name="request-2"></a><span data-ttu-id="b543b-201">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="b543b-201">Request 2</span></span>

<span data-ttu-id="b543b-p111">O segundo exemplo cria uma extensão na mensagem especificada. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="b543b-204">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="b543b-204">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b543b-205">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="b543b-205">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="b543b-206">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="b543b-206">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions

{ 
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension", 
  "extensionName" : "Com.Contoso.Referral", 
  "companyName" : "Wingtip Toys", 
  "dealValue" : 500050, 
  "expirationDate" : "2015-12-03T10:00:00.000Z" 
} 
```

##### <a name="response-2"></a><span data-ttu-id="b543b-207">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="b543b-207">Response 2</span></span>

<span data-ttu-id="b543b-p112">Veja a seguir a resposta para o segundo exemplo. O corpo da solicitação inclui o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="b543b-210">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="b543b-210">The default property **extensionName**.</span></span>
- <span data-ttu-id="b543b-211">A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="b543b-211">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span> 
- <span data-ttu-id="b543b-212">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="b543b-212">The custom data to be stored.</span></span>  

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

##### <a name="request-3"></a><span data-ttu-id="b543b-213">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="b543b-213">Request 3</span></span>

<span data-ttu-id="b543b-p113">O terceiro exemplo cria uma extensão no evento de grupo especificado. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="b543b-216">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="b543b-216">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b543b-217">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="b543b-217">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="b543b-218">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="b543b-218">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>  

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl17IsAAA=')/extensions 

{
  "@odata.type" : "Microsoft.Graph.OpenTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

##### <a name="response-3"></a><span data-ttu-id="b543b-219">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="b543b-219">Response 3</span></span>

<span data-ttu-id="b543b-220">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="b543b-220">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.opentypeextension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVl7IsAAA%3D')/extensions/$entity",
    "@odata.type": "#Microsoft.Graph.OpenTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Deal",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": 1010100,
    "expirationDate": "2015-07-03T13:04:00Z"
}
```

****

##### <a name="request-4"></a><span data-ttu-id="b543b-221">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="b543b-221">Request 4</span></span>

<span data-ttu-id="b543b-p114">O quarto exemplo cria uma extensão em uma nova postagem de grupo, usando a mesma chamada de ação **reply** para uma postagem de grupo existente. A ação **reply** cria uma nova postagem e uma nova extensão inserida nessa postagem. O corpo da solicitação inclui uma propriedade **post** que, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="b543b-225">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="b543b-225">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b543b-226">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="b543b-226">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="b543b-227">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="b543b-227">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA==')/posts('AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=')/microsoft.graph.reply 

{
  "post": {
    "body": {
      "contentType": "html",
      "content": "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  "extensions": [
    {
      "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
      "extensionName": "Com.Contoso.HR",
      "companyName": "Contoso",
      "expirationDate": "2015-07-03T13:04:00.000Z",
      "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]        
  }
}
```

##### <a name="response-4"></a><span data-ttu-id="b543b-228">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="b543b-228">Response 4</span></span>

<span data-ttu-id="b543b-p115">Veja a seguir a resposta do quarto exemplo. Criar uma extensão com êxito em uma nova postagem de grupo resulta apenas no código de resposta HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="b543b-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Content-type: text/plain
Content-Length: 0
```


****

##### <a name="request-5"></a><span data-ttu-id="b543b-231">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="b543b-231">Request 5</span></span>

<span data-ttu-id="b543b-p116">O quinto exemplo cria uma extensão em uma nova postagem de grupo usando a mesma operação POST para criar uma conversa. A operação POST cria uma nova conversa, thread ou postagem e uma nova extensão inserida na postagem. O corpo da solicitação inclui as propriedades **Topic** e **Threads** e o objeto filho **post** para a nova conversa. O objeto **post**, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a extensão:</span><span class="sxs-lookup"><span data-stu-id="b543b-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="b543b-236">O tipo `Microsoft.Graph.OpenTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="b543b-236">The type `Microsoft.Graph.OpenTypeExtension`.</span></span> 
- <span data-ttu-id="b543b-237">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="b543b-237">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="b543b-238">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="b543b-238">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations

{
  "Topic": "Does anyone have a second?",
  "Threads": [
    {
      "Posts": [
        {
          "Body": {
            "ContentType": "HTML",
            "Content": "This is urgent!"
          },
          "Extensions": [
            {
              "@odata.type": "Microsoft.OutlookServices.OpenTypeExtension",
              "extensionName": "Com.Contoso.Benefits",
              "companyName": "Contoso",
              "expirationDate": "2016-08-03T11:00:00.000Z",
              "topPicks": [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]  
            }  
          ] 
        } 
      ]  
    } 
  ]
}
```

##### <a name="response-5"></a><span data-ttu-id="b543b-239">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="b543b-239">Response 5</span></span>

<span data-ttu-id="b543b-p117">Veja a seguir a resposta do quinto exemplo, que contém a nova conversa e uma ID de thread. Esse novo thread contém uma postagem criada automaticamente que, por sua vez, contém a nova extensão.</span><span class="sxs-lookup"><span data-stu-id="b543b-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span> 

<span data-ttu-id="b543b-p118">Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b543b-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="b543b-p119">Para obter a nova extensão, primeiro [obtenha todas as postagens](../api/conversationthread_list_posts.md) desse thread. Inicialmente, deve haver somente uma. Em seguida, aplique a ID da postagem e o nome da extensão `Com.Contoso.Benefits` para [obter a extensão](../api/opentypeextension_get.md).</span><span class="sxs-lookup"><span data-stu-id="b543b-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations/$entity",
    "id": "AAQkADJToRlbJ5Mg7TFM7H-j3Y=",
    "threads@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/conversations('AAQkADJToRlbJ5Mg7TFM7H-j3Y%3D')/threads",
    "threads": [
        {
            "id": "AAQkADJDtMUzsf_PdhAAswJOhGVsnkyDtMUzsf_Pdg=="
        }
    ]
}

```


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
