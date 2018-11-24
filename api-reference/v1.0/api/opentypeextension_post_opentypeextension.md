# <a name="create-open-extension"></a><span data-ttu-id="08db6-101">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="08db6-101">Create open extension</span></span>

<span data-ttu-id="08db6-102">Crie uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso.</span><span class="sxs-lookup"><span data-stu-id="08db6-102">Create an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) and add custom properties in a new or existing instance of a resource.</span></span>

> <span data-ttu-id="08db6-103">**Observação:** Se você estiver criando extensões open nos recursos do Outlook, consulte **Considerações específicas do Outlook** em [tipo de recurso openTypeExtension](../resources/opentypeextension.md#outlook-specific-considerations).</span><span class="sxs-lookup"><span data-stu-id="08db6-103">**Note:** If you're creating open extensions on Outlook resources, see **Outlook-specific considerations** in [openTypeExtension resource type](../resources/opentypeextension.md#outlook-specific-considerations).</span></span>

## <a name="permissions"></a><span data-ttu-id="08db6-104">Permissions</span><span class="sxs-lookup"><span data-stu-id="08db6-104">Permissions</span></span>

<span data-ttu-id="08db6-105">Dependendo do recurso que você está criando a extensão na e a permissão tipo (delegado ou aplicativo) solicitada, a permissão especificada na tabela a seguir é o menos privilegiada necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="08db6-105">Depending on the resource you're creating the extension in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="08db6-106">Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="08db6-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="08db6-107">Recurso com suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-107">Supported resource</span></span> | <span data-ttu-id="08db6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08db6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="08db6-109">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08db6-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08db6-110">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08db6-110">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="08db6-111">device</span><span class="sxs-lookup"><span data-stu-id="08db6-111">device</span></span>](../resources/device.md) | <span data-ttu-id="08db6-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08db6-112">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="08db6-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-113">Not supported</span></span> | <span data-ttu-id="08db6-114">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-114">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="08db6-115">evento</span><span class="sxs-lookup"><span data-stu-id="08db6-115">event</span></span>](../resources/event.md) | <span data-ttu-id="08db6-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-116">Calendars.ReadWrite</span></span> | <span data-ttu-id="08db6-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-117">Calendars.ReadWrite</span></span> | <span data-ttu-id="08db6-118">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-118">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="08db6-119">grupo</span><span class="sxs-lookup"><span data-stu-id="08db6-119">group</span></span>](../resources/group.md) | <span data-ttu-id="08db6-120">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-120">Group.ReadWrite.All</span></span> | <span data-ttu-id="08db6-121">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-121">Not supported</span></span> | <span data-ttu-id="08db6-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-122">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="08db6-123">evento de grupo</span><span class="sxs-lookup"><span data-stu-id="08db6-123">group event</span></span>](../resources/event.md) | <span data-ttu-id="08db6-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="08db6-125">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-125">Not supported</span></span> | <span data-ttu-id="08db6-126">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-126">Not supported</span></span> |
| [<span data-ttu-id="08db6-127">postagem de grupo</span><span class="sxs-lookup"><span data-stu-id="08db6-127">group post</span></span>](../resources/post.md) | <span data-ttu-id="08db6-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="08db6-129">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-129">Not supported</span></span> | <span data-ttu-id="08db6-130">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-130">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="08db6-131">mensagem</span><span class="sxs-lookup"><span data-stu-id="08db6-131">message</span></span>](../resources/message.md) | <span data-ttu-id="08db6-132">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-132">Mail.ReadWrite</span></span> | <span data-ttu-id="08db6-133">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-133">Mail.ReadWrite</span></span> | <span data-ttu-id="08db6-134">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-134">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="08db6-135">organização</span><span class="sxs-lookup"><span data-stu-id="08db6-135">organization</span></span>](../resources/organization.md) | <span data-ttu-id="08db6-136">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="08db6-136">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="08db6-137">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-137">Not supported</span></span> | <span data-ttu-id="08db6-138">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-138">Not supported</span></span> |
| [<span data-ttu-id="08db6-139">contato pessoal</span><span class="sxs-lookup"><span data-stu-id="08db6-139">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="08db6-140">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-140">Contacts.ReadWrite</span></span> | <span data-ttu-id="08db6-141">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-141">Contacts.ReadWrite</span></span> | <span data-ttu-id="08db6-142">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-142">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="08db6-143">usuário</span><span class="sxs-lookup"><span data-stu-id="08db6-143">user</span></span>](../resources/user.md) | <span data-ttu-id="08db6-144">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-144">User.ReadWrite.All</span></span> | <span data-ttu-id="08db6-145">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08db6-145">User.ReadWrite</span></span> | <span data-ttu-id="08db6-146">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08db6-146">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08db6-147">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08db6-147">HTTP request</span></span>

### <a name="create-an-extension-in-a-new-resource-instance"></a><span data-ttu-id="08db6-148">Crie uma extensão em uma nova instância de recurso</span><span class="sxs-lookup"><span data-stu-id="08db6-148">Create an extension in a new resource instance</span></span>

<span data-ttu-id="08db6-149">Use a mesma solicitação REST que você usa para criar a instância.</span><span class="sxs-lookup"><span data-stu-id="08db6-149">Use the same REST request that you use to create the instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

><span data-ttu-id="08db6-150">**Observação:** Esta sintaxe mostra algumas maneiras comuns de criar as instâncias de recursos com suporte.</span><span class="sxs-lookup"><span data-stu-id="08db6-150">**Note:** This syntax shows some common ways to create the supported resource instances.</span></span> <span data-ttu-id="08db6-151">Todas as outras sintaxes POST que permite que você crie essas instâncias de recurso suporta as extensões de open criação de forma semelhante.</span><span class="sxs-lookup"><span data-stu-id="08db6-151">All other POST syntaxes that allows you to create these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="08db6-152">Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08db6-152">See the [Request body](#request-body) section about including the properties of the new resource instance _and the extension_ in the request body.</span></span>

### <a name="create-an-extension-in-an-existing-resource-instance"></a><span data-ttu-id="08db6-153">Crie uma extensão em uma instância de recurso existente</span><span class="sxs-lookup"><span data-stu-id="08db6-153">Create an extension in an existing resource instance</span></span>

<span data-ttu-id="08db6-154">Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.</span><span class="sxs-lookup"><span data-stu-id="08db6-154">Identify the resource instance in the request and do a `POST` to the **extensions** navigation property.</span></span>

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

><span data-ttu-id="08db6-155">**Observação:** Esta sintaxe mostra algumas maneiras comuns de identificar uma instância de recurso, para criar uma extensão nela.</span><span class="sxs-lookup"><span data-stu-id="08db6-155">**Note:** This syntax shows some common ways to identify a resource instance, in order to create an extension in it.</span></span> <span data-ttu-id="08db6-156">Oferece suporte a todas as outras sintaxes que permite que você identifique essas instâncias de recurso, Criando extensões open de forma semelhante.</span><span class="sxs-lookup"><span data-stu-id="08db6-156">All other syntaxes that allows you to identify these resource instances supports creating open extensions in them in a similar way.</span></span>

<span data-ttu-id="08db6-157">Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08db6-157">See the [Request body](#request-body) section about including _the extension_ in the request body.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="08db6-158">Parâmetros do caminho</span><span class="sxs-lookup"><span data-stu-id="08db6-158">Path parameters</span></span>
|<span data-ttu-id="08db6-159">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08db6-159">Parameter</span></span>|<span data-ttu-id="08db6-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="08db6-160">Type</span></span>|<span data-ttu-id="08db6-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="08db6-161">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="08db6-162">id</span><span class="sxs-lookup"><span data-stu-id="08db6-162">id</span></span>|<span data-ttu-id="08db6-163">string</span><span class="sxs-lookup"><span data-stu-id="08db6-163">string</span></span>|<span data-ttu-id="08db6-p104">Um identificador exclusivo para um objeto na coleção correspondente. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08db6-p104">A unique identifier for an object in the corresponding collection. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="08db6-166">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08db6-166">Request headers</span></span>

| <span data-ttu-id="08db6-167">Nome</span><span class="sxs-lookup"><span data-stu-id="08db6-167">Name</span></span>       | <span data-ttu-id="08db6-168">Valor</span><span class="sxs-lookup"><span data-stu-id="08db6-168">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="08db6-169">Autorização</span><span class="sxs-lookup"><span data-stu-id="08db6-169">Authorization</span></span> | <span data-ttu-id="08db6-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08db6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08db6-172">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08db6-172">Content-Type</span></span> | <span data-ttu-id="08db6-173">application/json</span><span class="sxs-lookup"><span data-stu-id="08db6-173">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08db6-174">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08db6-174">Request body</span></span>

<span data-ttu-id="08db6-p106">Forneça um corpo JSON de uma [openTypeExtension](../resources/openTypeExtension.md), com os seguintes pares de nome/valor obrigatórios e dados personalizados adicionais. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.</span><span class="sxs-lookup"><span data-stu-id="08db6-p106">Provide a JSON body of an [openTypeExtension](../resources/openTypeExtension.md), with the following required name-value pairs, and any additional custom data. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="08db6-177">Name</span><span class="sxs-lookup"><span data-stu-id="08db6-177">Name</span></span>       | <span data-ttu-id="08db6-178">Valor</span><span class="sxs-lookup"><span data-stu-id="08db6-178">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="08db6-179">@odata.type</span><span class="sxs-lookup"><span data-stu-id="08db6-179">@odata.type</span></span> | <span data-ttu-id="08db6-180">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="08db6-180">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="08db6-181">extensionName</span><span class="sxs-lookup"><span data-stu-id="08db6-181">extensionName</span></span> | <span data-ttu-id="08db6-182">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="08db6-182">%unique_string%</span></span> |

<span data-ttu-id="08db6-183">Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.</span><span class="sxs-lookup"><span data-stu-id="08db6-183">When creating an extension in a _new_ resource instance, in addition to the new **openTypeExtension** object, provide a JSON representation of the relevant properties to create such a resource instance.</span></span>

## <a name="response"></a><span data-ttu-id="08db6-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="08db6-184">Response</span></span>

### <a name="response-code"></a><span data-ttu-id="08db6-185">Código da resposta</span><span class="sxs-lookup"><span data-stu-id="08db6-185">Response code</span></span>

<span data-ttu-id="08db6-186">Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="08db6-186">Depending on the operation, the response code can be `201 Created` or `202 Accepted`.</span></span>

<span data-ttu-id="08db6-187">Quando você cria uma extensão usando a mesma operação que você pode usar para criar uma instância de recurso, a operação retorna o código de resposta mesmo que ele retorna ao usar a operação para criar a instância de recurso sem a extensão.</span><span class="sxs-lookup"><span data-stu-id="08db6-187">When you create an extension using the same operation that you use to create a resource instance, the operation returns the same response code that it returns when you use the operation to create the resource instance without the extension.</span></span>
<span data-ttu-id="08db6-188">Consulte os tópicos correspondentes para criar a instância, como listadas [acima](#create-an-extension-in-a-new-resource-instance).</span><span class="sxs-lookup"><span data-stu-id="08db6-188">Refer to the corresponding topics for creating the instance, as listed [above](#create-an-extension-in-a-new-resource-instance).</span></span>

### <a name="response-body"></a><span data-ttu-id="08db6-189">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="08db6-189">Response body</span></span>

| <span data-ttu-id="08db6-190">Cenário</span><span class="sxs-lookup"><span data-stu-id="08db6-190">Scenario</span></span>       | <span data-ttu-id="08db6-191">Recurso</span><span class="sxs-lookup"><span data-stu-id="08db6-191">Resource</span></span>  | <span data-ttu-id="08db6-192">Corpo da resposta</span><span class="sxs-lookup"><span data-stu-id="08db6-192">Response body</span></span> |
|:---------------|:----------|:--------------|
| <span data-ttu-id="08db6-193">Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso</span><span class="sxs-lookup"><span data-stu-id="08db6-193">Creating an extension while explicitly creating a _new_ resource instance</span></span> | <span data-ttu-id="08db6-194">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="08db6-194">[contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md)</span></span> | <span data-ttu-id="08db6-195">Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/openTypeExtension.md).</span><span class="sxs-lookup"><span data-stu-id="08db6-195">Includes the new instance expanded with the [openTypeExtension](../resources/openTypeExtension.md) object.</span></span> |
| <span data-ttu-id="08db6-196">Criando uma extensão ao criar implicitamente uma instância de recursos</span><span class="sxs-lookup"><span data-stu-id="08db6-196">Creating an extension while implicitly creating a resource instance</span></span> | [<span data-ttu-id="08db6-197">postagem</span><span class="sxs-lookup"><span data-stu-id="08db6-197">post</span></span>](../resources/post.md) | <span data-ttu-id="08db6-198">A resposta inclui somente um código de resposta, mas não um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08db6-198">The response includes only a response code but not a response body.</span></span> |
| <span data-ttu-id="08db6-199">Criar uma extensão em uma instância de recurso _existente_</span><span class="sxs-lookup"><span data-stu-id="08db6-199">Creating an extension in an _existing_ resource instance</span></span> | <span data-ttu-id="08db6-200">Todos os recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="08db6-200">All supported resources</span></span> | <span data-ttu-id="08db6-201">Inclui o objeto **openTypeExtension**.</span><span class="sxs-lookup"><span data-stu-id="08db6-201">Includes the **openTypeExtension** object.</span></span> |

## <a name="example"></a><span data-ttu-id="08db6-202">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08db6-202">Example</span></span>

### <a name="request-1"></a><span data-ttu-id="08db6-203">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="08db6-203">Request 1</span></span>

<span data-ttu-id="08db6-p108">O primeiro exemplo cria uma mensagem e uma extensão na mesma chamada. O corpo da solicitação inclui o seguinte:</span><span class="sxs-lookup"><span data-stu-id="08db6-p108">The first example creates a message and an extension in the same call. The request body includes the following:</span></span>

- <span data-ttu-id="08db6-206">As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem.</span><span class="sxs-lookup"><span data-stu-id="08db6-206">The **subject**, **body**, and **toRecipients** properties typical of a new message.</span></span>
- <span data-ttu-id="08db6-207">E para a extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-207">And for the extension:</span></span>

  - <span data-ttu-id="08db6-208">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="08db6-208">The type `microsoft.graph.openTypeExtension`.</span></span>
  - <span data-ttu-id="08db6-209">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="08db6-209">The extension name "Com.Contoso.Referral".</span></span>
  - <span data-ttu-id="08db6-210">Dados adicionais a serem armazenados como três propriedades personalizadas na carga JSON: `companyName`, `expirationDate`, e `dealValue`.</span><span class="sxs-lookup"><span data-stu-id="08db6-210">Additional data to be stored as three custom properties in the JSON payload: `companyName`, `expirationDate`, and `dealValue`.</span></span>

<!-- {
  "blockType": "ignored",
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
      "@odata.type": "microsoft.graph.openTypeExtension",
      "extensionName": "Com.Contoso.Referral",
      "companyName": "Wingtip Toys",
      "expirationDate": "2015-12-30T11:00:00.000Z",
      "dealValue": 10000
    }
  ]
}
```

### <a name="response-1"></a><span data-ttu-id="08db6-211">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="08db6-211">Response 1</span></span>

<span data-ttu-id="08db6-p109">Veja a seguir a resposta para o primeiro exemplo. O corpo da resposta inclui propriedades da nova mensagem e o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-p109">Here is the response for the first example. The response body includes properties of the new message, and the following for the new extension:</span></span>

- <span data-ttu-id="08db6-214">A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="08db6-214">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="08db6-215">A propriedade padrão **extensionName** especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="08db6-215">The default property **extensionName** specified in the request.</span></span>
- <span data-ttu-id="08db6-216">Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="08db6-216">The custom data specified in the request stored as 3 custom properties.</span></span>

<span data-ttu-id="08db6-p110">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08db6-p110">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.openTypeExtension",
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

### <a name="request-2"></a><span data-ttu-id="08db6-219">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="08db6-219">Request 2</span></span>

<span data-ttu-id="08db6-p111">O segundo exemplo cria uma extensão na mensagem especificada. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-p111">The second example creates an extension in the specified message. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="08db6-222">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="08db6-222">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="08db6-223">O nome da extensão "Com.Contoso.Referral".</span><span class="sxs-lookup"><span data-stu-id="08db6-223">The extension name "Com.Contoso.Referral".</span></span>
- <span data-ttu-id="08db6-224">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="08db6-224">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Referral",
  "companyName" : "Wingtip Toys",
  "dealValue" : 500050,
  "expirationDate" : "2015-12-03T10:00:00.000Z"
}
```

### <a name="response-2"></a><span data-ttu-id="08db6-225">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="08db6-225">Response 2</span></span>

<span data-ttu-id="08db6-p112">Veja a seguir a resposta para o segundo exemplo. O corpo da solicitação inclui o seguinte para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-p112">Here is the response for the second example. The response body includes the following for the new extension:</span></span>

- <span data-ttu-id="08db6-228">A propriedade padrão **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="08db6-228">The default property **extensionName**.</span></span>
- <span data-ttu-id="08db6-229">A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span><span class="sxs-lookup"><span data-stu-id="08db6-229">The **id** property with the fully qualified name of `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`.</span></span>
- <span data-ttu-id="08db6-230">Os dados personalizados a serem armazenados.</span><span class="sxs-lookup"><span data-stu-id="08db6-230">The custom data to be stored.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
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
    "expirationDate": "2015-12-03T10:00:00.000Z"
}
```

****

### <a name="request-3"></a><span data-ttu-id="08db6-231">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="08db6-231">Request 3</span></span>

<span data-ttu-id="08db6-p113">O terceiro exemplo cria uma extensão no evento de grupo especificado. O corpo da solicitação inclui o seguinte para essa extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-p113">The third example creates an extension in the specified group event. The request body includes the following for the extension:</span></span>

- <span data-ttu-id="08db6-234">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="08db6-234">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="08db6-235">O nome da extensão "Com.Contoso.Deal".</span><span class="sxs-lookup"><span data-stu-id="08db6-235">The extension name "Com.Contoso.Deal".</span></span>
- <span data-ttu-id="08db6-236">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.</span><span class="sxs-lookup"><span data-stu-id="08db6-236">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `dealValue`, and `expirationDate`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions

{
  "@odata.type" : "microsoft.graph.openTypeExtension",
  "extensionName" : "Com.Contoso.Deal",
  "companyName" : "Alpine Skis",
  "dealValue" : 1010100,
  "expirationDate" : "2015-07-03T13:04:00.000Z"
}
```

### <a name="response-3"></a><span data-ttu-id="08db6-237">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="08db6-237">Response 3</span></span>

<span data-ttu-id="08db6-238">Veja a seguir a resposta da terceira solicitação de exemplo.</span><span class="sxs-lookup"><span data-stu-id="08db6-238">Here is the response from the third example request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.openTypeExtension"
} -->
```http
HTTP/1.1 201 Created
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

### <a name="request-4"></a><span data-ttu-id="08db6-239">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="08db6-239">Request 4</span></span>

<span data-ttu-id="08db6-p114">O quarto exemplo cria uma extensão em uma nova postagem de grupo, usando a mesma chamada de ação **reply** para uma postagem de grupo existente. A ação **reply** cria uma nova postagem e uma nova extensão inserida nessa postagem. O corpo da solicitação inclui uma propriedade **post** que, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a nova extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-p114">The fourth example creates an extension in a new group post, using the same **reply** action call to an existing group post. The **reply** action creates a new post, and a new extension embedded in the post. The request body includes a **post** property, which in turn contains the **body** of the new post, and the following data for the new extension:</span></span>

- <span data-ttu-id="08db6-243">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="08db6-243">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="08db6-244">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="08db6-244">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="08db6-245">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="08db6-245">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_4"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply

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

### <a name="response-4"></a><span data-ttu-id="08db6-246">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="08db6-246">Response 4</span></span>

<span data-ttu-id="08db6-p115">Veja a seguir a resposta do quarto exemplo. Criar uma extensão com êxito em uma nova postagem de grupo resulta apenas no código de resposta HTTP 202.</span><span class="sxs-lookup"><span data-stu-id="08db6-p115">Here is the response from the fourth example. Successfully creating an extension in a new group post results in only the HTTP 202 response code.</span></span>

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

### <a name="request-5"></a><span data-ttu-id="08db6-249">Solicitação 5</span><span class="sxs-lookup"><span data-stu-id="08db6-249">Request 5</span></span>

<span data-ttu-id="08db6-p116">O quinto exemplo cria uma extensão em uma nova postagem de grupo usando a mesma operação POST para criar uma conversa. A operação POST cria uma nova conversa, thread ou postagem e uma nova extensão inserida na postagem. O corpo da solicitação inclui as propriedades **Topic** e **Threads** e o objeto filho **post** para a nova conversa. O objeto **post**, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a extensão:</span><span class="sxs-lookup"><span data-stu-id="08db6-p116">The fifth example creates an extension in a new group post using the same POST operation to create a conversation. The POST operation creates a new conversation, thread and post, and a new extension embedded in the post. The request body includes the **Topic** and **Threads** properties, and a child **post** object for the new conversation. The **post** object in turn contains the **body** of the new post, and the following data for the extension:</span></span>

- <span data-ttu-id="08db6-254">O tipo `microsoft.graph.openTypeExtension`.</span><span class="sxs-lookup"><span data-stu-id="08db6-254">The type `microsoft.graph.openTypeExtension`.</span></span>
- <span data-ttu-id="08db6-255">O nome da extensão "Com.Contoso.HR".</span><span class="sxs-lookup"><span data-stu-id="08db6-255">The extension name "Com.Contoso.HR".</span></span>
- <span data-ttu-id="08db6-256">Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.</span><span class="sxs-lookup"><span data-stu-id="08db6-256">Additional data to be stored as 3 custom properties in the JSON payload: `companyName`, `expirationDate`, and the array of strings `topPicks`.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "post_opentypeextension_5"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations

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

### <a name="response-5"></a><span data-ttu-id="08db6-257">Resposta 5</span><span class="sxs-lookup"><span data-stu-id="08db6-257">Response 5</span></span>

<span data-ttu-id="08db6-p117">Veja a seguir a resposta do quinto exemplo, que contém a nova conversa e uma ID de thread. Esse novo thread contém uma postagem criada automaticamente que, por sua vez, contém a nova extensão.</span><span class="sxs-lookup"><span data-stu-id="08db6-p117">Here is the response from the fifth example which contains the new conversation and a thread ID. This new thread contains an automatically created post, which in turn contains the new extension.</span></span>

<span data-ttu-id="08db6-p118">Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08db6-p118">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<span data-ttu-id="08db6-p119">Para obter a nova extensão, primeiro [obtenha todas as postagens](../api/conversationthread_list_posts.md) desse thread. Inicialmente, deve haver somente uma. Em seguida, aplique a ID da postagem e o nome da extensão `Com.Contoso.Benefits` para [obter a extensão](../api/opentypeextension_get.md).</span><span class="sxs-lookup"><span data-stu-id="08db6-p119">To get the new extension, first [get all the posts](../api/conversationthread_list_posts.md) in this thread, and initially there should be only one. Then apply the post ID and the extension name `Com.Contoso.Benefits` to [get the extension](../api/opentypeextension_get.md).</span></span>

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
