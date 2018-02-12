# <a name="add-custom-data-to-groups-using-schema-extensions"></a><span data-ttu-id="a014c-101">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="a014c-101">Add custom data to groups using schema extensions</span></span> 

<span data-ttu-id="a014c-102">Por meio de um exemplo, vamos demonstrar como usar as *extensões de esquema*.</span><span class="sxs-lookup"><span data-stu-id="a014c-102">We're going to walk you through an example to demonstrate how to use *schema extensions*.</span></span> 

<span data-ttu-id="a014c-p101">Imagine que você é um desenvolvedor em uma empresa de Software de gerenciamento de aprendizagem chamada “Graph Learn” que cria cursos e materiais de treinamento para empresas.  Os grupos do Office 365, com experiências colaborativas avançadas, são uma maneira fantástica de fornecer o conteúdo do curso e gravar exercícios entre os participantes de cursos online e presenciais.  Talvez você deseje deixar os grupos do Office 365 usados para cursos de treinamento facilmente identificados como cursos de treinamento, pois isso permite que outros desenvolvedores descubram seus grupos e criem experiências avançadas com base nos seus cursos de treinamento.</span><span class="sxs-lookup"><span data-stu-id="a014c-p101">Imagine you're a developer in a Learning Management Software company called “Graph Learn” that builds training courses and materials for businesses.  Office 365 groups, with their rich collaborative experiences, is a fantastic way to deliver course content and record exercises among participants for both online courses and instructor-led courses.  You may want to make those Office 365 groups used for training courses easily identifiable as training courses, which will allow other developers to discover your groups and build rich experiences on top of your learning courses.</span></span>

<span data-ttu-id="a014c-106">Neste cenário, vamos mostrar como:</span><span class="sxs-lookup"><span data-stu-id="a014c-106">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="a014c-107">Exibir definições de extensão de esquema disponíveis que você poderia usar.</span><span class="sxs-lookup"><span data-stu-id="a014c-107">View available schema extension definitions that you could use.</span></span>
2. <span data-ttu-id="a014c-108">Registrar uma definição de extensão de esquema direcionada a grupos de cursos de treinamento.</span><span class="sxs-lookup"><span data-stu-id="a014c-108">Register a schema extension definition that targets groups for training courses.</span></span>
3. <span data-ttu-id="a014c-109">Criar um novo grupo com dados estendidos baseados na definição de extensão do esquema que você acabou de registrar.</span><span class="sxs-lookup"><span data-stu-id="a014c-109">Create a new group with extended data based on the schema extension definition that you just registered.</span></span>
4. <span data-ttu-id="a014c-110">Adicionar, atualizar ou remover dados personalizados em um grupo existente com base em uma definição de extensão de esquema.</span><span class="sxs-lookup"><span data-stu-id="a014c-110">Add, update, or remove custom data in an existing group based on a schema extension definition.</span></span>
5. <span data-ttu-id="a014c-111">Ler novamente um grupo e os dados de extensão.</span><span class="sxs-lookup"><span data-stu-id="a014c-111">Read back a group and the extension data.</span></span>

><span data-ttu-id="a014c-p102">**Observação:** Este tópico mostra como criar e ler valores de extensão do esquema em um recurso **group** (etapas 3 a 5).  Os mesmos métodos são compatíveis também com os tipos de recurso **administrativeUnit**, **device**, **event**, **message**, **organization**, **post** e **user**.  Portanto, você pode executar operações semelhantes às solicitações de exemplo abaixo em qualquer um desses recursos. Observe que **administrativeUnit** está disponível apenas no ponto de extremidade beta.</span><span class="sxs-lookup"><span data-stu-id="a014c-p102">**Note:** This topic shows you how to create and read schema extension values on a **group** resource (steps 3-5).  The same methods are supported for the **administrativeUnit**, **device**, **event**, **message**, **organization**, **post**, and **user** resource types as well.  So you can carry out similar operations as the example requests below on any of those resources. Note that **administrativeUnit** is available only in the beta endpoint.</span></span>

## <a name="1-view-available-schema-extensions"></a><span data-ttu-id="a014c-116">1. Exibir extensões de esquema disponíveis</span><span class="sxs-lookup"><span data-stu-id="a014c-116">1. View available schema extensions</span></span>
<span data-ttu-id="a014c-p103">Em primeiro lugar, como desenvolvedor, talvez seja interessante localizar todas as outras definições de extensão de esquema que nosso aplicativo possa reutilizar.  Isso pode ser feito consultando o recurso **schemaExtension**.</span><span class="sxs-lookup"><span data-stu-id="a014c-p103">First, as a developer, you might want to find any other schema extension definitions that our app could reuse.  This can be done by querying the **schemaExtension** resource.</span></span>  
<span data-ttu-id="a014c-119">No exemplo abaixo, você consultará uma extensão de esquema específica por **id**.</span><span class="sxs-lookup"><span data-stu-id="a014c-119">In the example below, you're going to query for a specific schema extension by **id**.</span></span>

<span data-ttu-id="a014c-p104">Observe que a extensão retornada na resposta tem **Disponível** como o valor de **status**, que indica que qualquer aplicativo que tem permissão para os recursos na propriedade **targetTypes** pode usar e atualizar a extensão com alterações aditivas. Em geral, essa operação retorna quaisquer extensões de esquema que satisfaçam ao filtro especificado independentemente do **status**. Portanto, verifique o status da extensão antes de usá-la.</span><span class="sxs-lookup"><span data-stu-id="a014c-p104">Notice that the extension returned in the response has **Available** as the **status** value, which indicates that any app which has permission to the resources in the **targetTypes** property can use and update the extension with additive changes. In general, this operation returns any schema extensions that satisfy the specified filter regardless of **status**, so do check the extension status before using it.</span></span>


##### <a name="request"></a><span data-ttu-id="a014c-122">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a014c-122">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="a014c-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="a014c-123">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
            "owner": "24d3b144-21ae-4080-943f-7067b395b913",
            "properties": [
                {
                    "name": "testName",
                    "type": "String"
                }
            ]
        }
    ]
}
```
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a><span data-ttu-id="a014c-124">2. Registrar uma definição de extensão de esquema que descreve um grupo de treinamento</span><span class="sxs-lookup"><span data-stu-id="a014c-124">2. Register a schema extension definition that describes a training course</span></span>
<span data-ttu-id="a014c-125">Se não conseguir localizar uma extensão de esquema que *é* apropriada para suas necessidades, você poderá criar e registrar uma nova definição de extensão para cursos de treinamento no recurso **group**.</span><span class="sxs-lookup"><span data-stu-id="a014c-125">If you can't find a schema extension that *is* appropriate for your needs, you can create and register a new extension definition for training courses on the **group** resource.</span></span>  

<span data-ttu-id="a014c-p105">Ao criar uma definição de extensão de esquema, você deve fornecer uma cadeia de caracteres para a propriedade **id**. Há duas maneiras de se fazer isso. O exemplo a seguir mostra o método preferencial, que usa um nome de domínio personalizado (`graphlearn.com`) que foi verificado com seu locatário. Concatene o nome de domínio verificado (`graphlearn`) com um nome para a extensão de esquema (`courses`) e atribua **id** com a cadeia de caracteres resultante, `graphlearn_courses`.</span><span class="sxs-lookup"><span data-stu-id="a014c-p105">When creating a schema extension definition, you should provide a string for the **id** property. There are two ways to do this. The following example shows the preferred way, which uses a vanity domain name (`graphlearn.com`) that has been verified with your tenant. Concatenate the verified domain name (`graphlearn`) with a name for the schema extension (`courses`), and assign **id** with the resultant string, `graphlearn_courses`.</span></span>  

<span data-ttu-id="a014c-p106">Então especifique também uma descrição (para habilitar a capacidade de descoberta), tipos de destino (definindo a quais recursos essa extensão se aplica) e as propriedades personalizadas que compõem o esquema.  Neste exemplo, especifique as propriedades `courseId`, `courseName` e `courseType` personalizadas e seus tipos.</span><span class="sxs-lookup"><span data-stu-id="a014c-p106">Then, specify a description (to enable discoverability), target types (defining which resources this extension applies to), and the custom properties that make up the schema.  In this example, specify the `courseId`, `courseName` and `courseType` custom properties and their types.</span></span>

<span data-ttu-id="a014c-132">Veja um [exemplo de outra maneira de atribuir a **id** na solicitação](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md#request-2), que exige que você forneça apenas um nome de esquema.</span><span class="sxs-lookup"><span data-stu-id="a014c-132">See an [example of the other way to assign **id** in the request](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md#request-2), that requires you to provide only a schema name.</span></span>

<span data-ttu-id="a014c-p107">Observe que, quando você cria uma extensão de esquema inicialmente, seu status é **InDevelopment**. Ao desenvolver a extensão, você pode mantê-la com esse status. Enquanto isso, apenas seu aplicativo que a criou pode atualizá-la com alterações aditivas ou excluí-la. Quando estiver pronto para compartilhar a extensão para uso por outros aplicativos, defina o **status** como **Disponível**.</span><span class="sxs-lookup"><span data-stu-id="a014c-p107">Notice that when you initially create a schema extension, its status is **InDevelopment**. While you're developing the extension, you can keep it in this status, during which only your app that created it can update it with additive changes or delete it. When you are ready to share the extension for use by other apps, set **status** to **Available**.</span></span>

##### <a name="request"></a><span data-ttu-id="a014c-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a014c-136">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="a014c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a014c-137">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
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

## <a name="3-create-a-new-group-with-extended-data"></a><span data-ttu-id="a014c-138">3. Criar um novo grupo com dados estendidos</span><span class="sxs-lookup"><span data-stu-id="a014c-138">3. Create a new group with extended data</span></span> 
<span data-ttu-id="a014c-p108">Criar um _novo_ grupo estendido com dados extras usando a definição de extensão de esquema `graphlearn_courses` que acabamos de registrar.  Este é um padrão ```POST``` para o recurso **group**, com a extensão de tipo complexo `graphlearn_courses` definida no corpo da solicitação.  A resposta não refletirá extensões de dados. Precisamos explicitamente usar a extensão ```$select``` por nome usando uma operação ```GET```.</span><span class="sxs-lookup"><span data-stu-id="a014c-p108">Create a _new_ group and extend it with extra data using the `graphlearn_courses` schema extension definition that we just registered.  This is a standard ```POST``` to the **group** resource, with the additional `graphlearn_courses` complex type extension defined in the request body.  The response will not mirror back any data extensions. We need to explicitly ```$select``` the extension by name using a ```GET``` operation.</span></span>

##### <a name="request"></a><span data-ttu-id="a014c-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a014c-143">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a><span data-ttu-id="a014c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a014c-144">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a><span data-ttu-id="a014c-145">4. Adicionar, atualizar ou remover dados personalizados em um grupo existente</span><span class="sxs-lookup"><span data-stu-id="a014c-145">4. Add, update, or remove custom data in an existing group</span></span>
<span data-ttu-id="a014c-146">Você pode estender e adicionar dados personalizados a uma instância de grupo _existente_ a extensão de tipo complexo `graphlearn_courses` adicional no corpo de uma solicitação ```PATCH```.</span><span class="sxs-lookup"><span data-stu-id="a014c-146">You can extend and add custom data to an _existing_ group instance with the additional `graphlearn_courses` complex type extension defined in the body of a ```PATCH``` request.</span></span>  

##### <a name="request"></a><span data-ttu-id="a014c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a014c-147">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a><span data-ttu-id="a014c-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a014c-148">Response</span></span>
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="a014c-149">Se você quiser atualizar os valores dos dados de extensão, coloque todo o tipo complexo de extensão no corpo de uma solicitação ```PATCH``` (semelhante a adicionar dados personalizados a um recurso existente).</span><span class="sxs-lookup"><span data-stu-id="a014c-149">If you want to update the values of the extension data, put the entire extension complex type in the body of a ```PATCH``` request (similar to adding custom data to an existing resource).</span></span>

<span data-ttu-id="a014c-150">Você também pode remover dados personalizados adicionados a uma instância de recursos, definindo a propriedade de extensão correspondente como nulo.</span><span class="sxs-lookup"><span data-stu-id="a014c-150">You can also remove custom data added to a resource instance by setting the corresponding extension property to null.</span></span> 

<span data-ttu-id="a014c-151">Para remover uma extensão de esquema de uma instância do recurso, defina o tipo complexo da extensão dessa instância como nulo.</span><span class="sxs-lookup"><span data-stu-id="a014c-151">To remove a schema extension from a resource instance, set the extension complex type in that instance to null.</span></span>


## <a name="5-get-a-group-and-its-extension-data"></a><span data-ttu-id="a014c-152">5. Obter um grupo e seus dados de extensão</span><span class="sxs-lookup"><span data-stu-id="a014c-152">5. Get a group and its extension data</span></span>
<span data-ttu-id="a014c-153">Uma maneira conveniente de procurar um grupo (ou grupos) é usar `$filter` para corresponder a valores de propriedades de extensão específica, como um nome de extensão ou ID.</span><span class="sxs-lookup"><span data-stu-id="a014c-153">A handy way to look for a group (or groups) is to use `$filter` to match for specific extension property values, such as an extension name or ID.</span></span> 

<span data-ttu-id="a014c-154">Então, para obter os dados personalizados em um grupo, use `$select` para incluir a extensão de nome (neste caso, `graphlearn_courses`).</span><span class="sxs-lookup"><span data-stu-id="a014c-154">Then, to get the custom data in a group, use `$select` to include the extension by name (in this case by `graphlearn_courses`).</span></span>

<span data-ttu-id="a014c-p109">O exemplo a seguir procura o grupo que possui a extensão `graphlearn_courses` com um valor de propriedade `courseId` correspondente a `123` e obtém as propriedades do grupo **displayName**, **id** e **description** e os dados personalizados na extensão `graphlearn_courses`. (Na consulta em si, certifique-se de aplicar codificação de URL conforme necessário).</span><span class="sxs-lookup"><span data-stu-id="a014c-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

#### <a name="request"></a><span data-ttu-id="a014c-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a014c-157">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a><span data-ttu-id="a014c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="a014c-158">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="a014c-159">Veja também</span><span class="sxs-lookup"><span data-stu-id="a014c-159">See also</span></span>

- [<span data-ttu-id="a014c-160">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a014c-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="a014c-161">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="a014c-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- [<span data-ttu-id="a014c-162">Domínios do Office 365</span><span class="sxs-lookup"><span data-stu-id="a014c-162">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)
- [<span data-ttu-id="a014c-163">Adicionando e verificando um domínio para o NOVO Office 365</span><span class="sxs-lookup"><span data-stu-id="a014c-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="a014c-164">Tipo de recurso schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a014c-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="a014c-165">List schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="a014c-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="a014c-166">Create schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a014c-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="a014c-167">Get schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a014c-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="a014c-168">Update schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a014c-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="a014c-169">Delete schemaExtension</span><span class="sxs-lookup"><span data-stu-id="a014c-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)
