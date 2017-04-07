# <a name="add-custom-data-to-groups-using-schema-extensions-preview"></a>Adicionar dados personalizados a grupos usando extensões do esquema (visualização)

Por meio de um exemplo, vamos demonstrar como usar as *extensões de esquema*. 

Imagine que você é um desenvolvedor em uma empresa de Software de gerenciamento de aprendizagem chamada “Graph Learn” que cria cursos e materiais de treinamento para empresas.  Os grupos do Office 365, com experiências colaborativas avançadas, são uma maneira fantástica de fornecer o conteúdo do curso e gravar exercícios entre os participantes de cursos online e presenciais.  Talvez você deseje deixar os grupos do Office 365 usados para cursos de treinamento facilmente identificados como cursos de treinamento, pois isso permite que outros desenvolvedores descubram seus grupos e criem experiências avançadas com base nos seus cursos de treinamento.

Neste cenário, vamos mostrar como:

1. Exibir definições de extensão de esquema disponíveis que você poderia usar
2. Registrar uma definição de extensão de esquema direcionada a grupos de cursos de treinamento
3. Criar um novo grupo com dados estendidos baseados na definição de extensão do esquema que você acabou de registrar
4. Adicionar ou atualizar dados personalizados a um grupo existente com base em uma definição de extensão de esquema
5. Ler novamente um grupo e os dados de extensão

>**Observação:** Este tópico mostra como criar e ler valores de extensão do esquema em um recurso **group** (etapas 3 a 5).  Os mesmos métodos também têm suporte para os tipos de recursos **device**, **event**, **message**, **post** e **user**.  Portanto, você pode executar operações semelhantes às solicitações de exemplo abaixo em qualquer um desses recursos.

## <a name="1-view-available-schema-extensions"></a>1. Exibir extensões de esquema disponíveis
Em primeiro lugar, como desenvolvedor, talvez seja interessante localizar todas as outras definições de extensão de esquema que nosso aplicativo possa reutilizar.  Isso pode ser feito consultando o recurso **schemaExtension**.  
No exemplo abaixo, você consultará uma extensão de esquema específica por **id**.

Observe que a extensão retornada na resposta tem **Disponível** como o valor de **status**, que indica que qualquer aplicativo que tem permissão para os recursos na propriedade **targetTypes** pode usar e atualizar a extensão com alterações aditivas. Em geral, essa operação retorna quaisquer extensões de esquema que satisfaçam ao filtro especificado independentemente do **status**. Portanto, verifique o status da extensão antes de usá-la.


##### <a name="request"></a>Solicitação
```http
GET https://graph.microsoft.com/beta/schemaExtensions/$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a>Resposta
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
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a>2. Registrar uma definição de extensão de esquema que descreve um grupo de treinamento
Se não conseguir localizar uma extensão de esquema que *é* apropriada para suas necessidades, você poderá criar e registrar uma nova definição de extensão para cursos de treinamento no recurso **group**.  

Ao criar uma definição de extensão de esquema, você deve fornecer uma cadeia de caracteres para a propriedade **id**. Há duas maneiras de se fazer isso. O exemplo a seguir mostra o método preferencial, que usa um nome de domínio personalizado (`graphlearn.com`) que foi verificado com seu locatário. Concatene o nome de domínio verificado (`graphlearn`) com um nome para a extensão de esquema (`courses`) e atribua **id** com a cadeia de caracteres resultante, `graphlearn_courses`.  Especifique também uma descrição (para habilitar a capacidade de descoberta), tipos de destino (definindo a quais recursos essa extensão se aplica) e as propriedades personalizadas que compõem o esquema.  Neste exemplo, especifique as propriedades personalizadas `courseId`, `courseName` e `courseType` e seus tipos.

Veja um [exemplo de outra maneira de atribuir a **id** na solicitação](../api-reference/beta/api/schemaextension_post_schemaextensions.md#request-2), que exige que você forneça apenas um nome de esquema.

Observe que, quando você cria uma extensão de esquema inicialmente, seu status é **InDevelopment**. Ao desenvolver a extensão, você pode mantê-la com esse status. Enquanto isso, apenas seu aplicativo que a criou pode atualizá-la com alterações aditivas ou excluí-la. Quando estiver pronto para compartilhar a extensão para uso por outros aplicativos, defina o **status** como **Disponível**.

##### <a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/beta/schemaExtensions
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
##### <a name="response"></a>Resposta
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "graphlearn_course",
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

## <a name="3-create-a-new-group-with-extended-data"></a>3. Criar um novo grupo com dados estendidos 
Criar um novo grupo estendido com dados extras usando a definição de extensão de esquema `graphlearn_courses` que acabamos de registrar.  Este é um padrão ```POST``` para o recurso **group**, com a extensão de tipo complexo `graphlearn_courses` definida no corpo da solicitação.  A resposta não refletirá extensões de dados. Precisamos explicitamente usar a extensão ```$select``` por nome usando uma operação ```GET```.

##### <a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/beta/groups
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
##### <a name="response"></a>Resposta
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

## <a name="4-add-or-update-custom-data-to-an-existing-group"></a>4. Adicionar ou atualizar dados personalizados a um grupo existente
De forma semelhante ao último exemplo, podemos estender um recurso de grupo existente com a extensão de tipo complexo `graphlearn_courses` adicional definida no corpo de uma solicitação ```PATCH```.  

##### <a name="request"></a>Solicitação
```http
PATCH https://graph.microsoft.com/beta/groups/dfc8016f-db97-4c47-a582-49cb8f849355
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
##### <a name="response"></a>Resposta
```http
HTTP/1.1 204 No Content
```

Se você quiser atualizar os valores dos dados de extensão, coloque todo o tipo complexo de extensão no corpo de uma solicitação ```PATCH``` (semelhante a adicionar dados personalizados a um recurso existente).

## <a name="5-get-a-group-and-its-extension-data"></a>5. Obter um grupo e seus dados de extensão
Para obter o grupo **e** seus dados de extensão, precisamos usar `$select` para especificar a extensão por nome, nesse caso, `graphlearn_courses`.

#### <a name="request"></a>Solicitação
```http
GET https://graph.microsoft.com/beta/groups/dfc8016f-db97-4c47-a582-49cb8f849355?$select=displayName,id,description,graphlearn_courses
```

##### <a name="response"></a>Resposta
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```

## <a name="see-also"></a>Ver também

- [Adicionar dados personalizados a recursos usando extensões](extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](extensibility_open_users.md)
- [Domínios do Office 365](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)
- [Adicionando e verificando um domínio para o NOVO Office 365](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [Tipo de recurso schemaExtension](../api-reference/beta/resources/schemaextension.md)
- [Listar schemaExtensions](../api-reference/beta/api/schemaextension_list.md)
- [Criar schemaExtension](../api-reference/beta/api/schemaextension_post_schemaextensions.md)
- [Obter schemaExtension](../api-reference/beta/api/schemaextension_get.md)
- [Atualizar schemaExtension](../api-reference/beta/api/schemaextension_update.md)
- [Excluir schemaExtension](../api-reference/beta/api/schemaextension_delete.md))
