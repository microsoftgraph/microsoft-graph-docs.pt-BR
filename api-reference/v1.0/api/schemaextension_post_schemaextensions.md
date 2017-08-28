# <a name="create-schemaextension"></a><span data-ttu-id="9df8e-101">Criar schemaExtension</span><span class="sxs-lookup"><span data-stu-id="9df8e-101">Create schemaExtension</span></span>

<span data-ttu-id="9df8e-102">Criar uma nova definição [schemaExtension](../resources/schemaextension.md) para estender um [tipo de recurso de suporte](../../../concepts/extensibility_overview.md#supported-resources).</span><span class="sxs-lookup"><span data-stu-id="9df8e-102">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="9df8e-p101">As extensões de esquema permitem que você adicione dados personalizados fortemente tipados a um recurso. O aplicativo que cria uma extensão de esquema é o aplicativo proprietário. Dependendo do [estado](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle) da extensão, o aplicativo proprietário, e apenas o aplicativo proprietário, poderá atualizar ou excluir a extensão.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="9df8e-106">Veja exemplos de como [definir uma extensão de esquema que descreve um curso de treinamento](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course), usar a definição de extensão do esquema para [criar um novo grupo com dados do curso de treinamento](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data) e [adicionar dados do curso de treinamento a um grupo existente](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group).</span><span class="sxs-lookup"><span data-stu-id="9df8e-106">See examples of how to [define a schema extension that describes a training course](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="9df8e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="9df8e-107">Permissions</span></span>
<span data-ttu-id="9df8e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9df8e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="9df8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9df8e-110">Permission type</span></span>      | <span data-ttu-id="9df8e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9df8e-111">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="9df8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9df8e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9df8e-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9df8e-113">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="9df8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9df8e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9df8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9df8e-115">Not supported.</span></span>    | 
|<span data-ttu-id="9df8e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9df8e-116">Application</span></span> | <span data-ttu-id="9df8e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9df8e-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9df8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9df8e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="9df8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9df8e-119">Request headers</span></span>
| <span data-ttu-id="9df8e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="9df8e-120">Name</span></span>       | <span data-ttu-id="9df8e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9df8e-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9df8e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9df8e-122">Authorization</span></span>  | <span data-ttu-id="9df8e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9df8e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9df8e-125">Content-Type</span></span>  | <span data-ttu-id="9df8e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9df8e-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9df8e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9df8e-127">Request body</span></span>
<span data-ttu-id="9df8e-128">No corpo da solicitação, forneça uma representação JSON de um objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="9df8e-128">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="9df8e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar uma extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="9df8e-129">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="9df8e-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9df8e-130">Parameter</span></span> | <span data-ttu-id="9df8e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9df8e-131">Type</span></span> | <span data-ttu-id="9df8e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9df8e-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9df8e-133">description</span><span class="sxs-lookup"><span data-stu-id="9df8e-133">description</span></span>|<span data-ttu-id="9df8e-134">String</span><span class="sxs-lookup"><span data-stu-id="9df8e-134">String</span></span>|<span data-ttu-id="9df8e-135">Descrição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="9df8e-135">Description for the schema extension.</span></span>|
|<span data-ttu-id="9df8e-136">id</span><span class="sxs-lookup"><span data-stu-id="9df8e-136">id</span></span>|<span data-ttu-id="9df8e-137">String</span><span class="sxs-lookup"><span data-stu-id="9df8e-137">String</span></span>|<span data-ttu-id="9df8e-138">O identificador exclusivo da definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="9df8e-138">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="9df8e-139">Você pode atribuir um valor em uma destas duas maneiras:</span><span class="sxs-lookup"><span data-stu-id="9df8e-139">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="9df8e-p104">Concatenar o nome de um de seus domínios verificados com um nome da extensão do esquema para formar uma cadeia de caracteres exclusiva neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Como exemplo, `contoso_mySchema`. </span><span class="sxs-lookup"><span data-stu-id="9df8e-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="9df8e-p105">Forneça um nome de esquema e permita que o Microsoft Graph use esse nome de esquema para completar a atribuição de **id** neste formato: ext\{_&#65279;8-caracteres-alfanuméricos-aleatórios_\}\_\{_&#65279;nome-do-esquema_\}. Um exemplo seria `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="9df8e-144">Esta propriedade não pode ser alterada após a criação.</span><span class="sxs-lookup"><span data-stu-id="9df8e-144">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="9df8e-145">propriedades</span><span class="sxs-lookup"><span data-stu-id="9df8e-145">properties</span></span>|<span data-ttu-id="9df8e-146">Coleção [extensionSchemaProperty](../resources/extensionschemaproperty.md)</span><span class="sxs-lookup"><span data-stu-id="9df8e-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="9df8e-147">A coleção de tipos e nomes de propriedades que compõem a definição da extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="9df8e-147">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="9df8e-148">targetTypes</span><span class="sxs-lookup"><span data-stu-id="9df8e-148">targetTypes</span></span>|<span data-ttu-id="9df8e-149">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9df8e-149">String collection</span></span>|<span data-ttu-id="9df8e-150">O conjunto de tipos de recursos do Microsoft Graph (com suporte a extensões do esquema) ao qual esta extensão de esquema pode ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="9df8e-150">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="9df8e-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9df8e-151">Response</span></span>

<span data-ttu-id="9df8e-152">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9df8e-152">If successful, this method returns `201, Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9df8e-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9df8e-153">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="9df8e-154">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="9df8e-154">Request 1</span></span>

<span data-ttu-id="9df8e-p106">O primeiro exemplo mostra o uso de um nome de domínio verificado, `graphlearn` e um nome de esquema, `courses`, para formar uma cadeia de caracteres para a propriedade **id** da definição de extensão do esquema. A cadeia de caracteres exclusiva se baseia neste formato, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p106">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="9df8e-157">No corpo da solicitação, forneça uma representação JSON do objeto [schemaExtension](../resources/schemaextension.md).</span><span class="sxs-lookup"><span data-stu-id="9df8e-157">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-1"></a><span data-ttu-id="9df8e-158">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="9df8e-158">Response 1</span></span>

<span data-ttu-id="9df8e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="9df8e-162">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="9df8e-162">Request 2</span></span>

<span data-ttu-id="9df8e-p108">O segundo exemplo mostra a especificação de apenas um nome de esquema, `courses`, na propriedade **id** na solicitação, junto com a representação JSON do resto das propriedades no objeto [schemaExtension](../resources/schemaextension.md). O Microsoft Graph atribuirá e retornará um valor exclusivo de cadeia de caracteres na resposta.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p108">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-2"></a><span data-ttu-id="9df8e-165">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="9df8e-165">Response 2</span></span>

<span data-ttu-id="9df8e-p109">A resposta inclui uma cadeia de caracteres exclusiva na propriedade **id** com base no nome do esquema fornecido na solicitação, junto com o resto da definição de esquema recém-criada. O valor em **id** na resposta se baseia no formato, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9df8e-p109">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="9df8e-170">Confira também</span><span class="sxs-lookup"><span data-stu-id="9df8e-170">See also</span></span>

- [<span data-ttu-id="9df8e-171">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="9df8e-171">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="9df8e-172">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="9df8e-172">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->