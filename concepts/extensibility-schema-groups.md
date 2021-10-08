---
title: 'Adicionar dados personalizados a grupos usando as extensões do esquema '
description: 'Este artigo apresenta um exemplo para demonstrar como usar *extensões de esquema*. '
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: c4226a642c2e6651cf4168c81d7188f0edd76270
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240653"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a>Adicionar dados personalizados a grupos usando as extensões do esquema 

Este artigo apresenta um exemplo para demonstrar como usar *extensões de esquema*. 

Imagine que você é um desenvolvedor em uma empresa de Software de gestão escolar chamada “Graph Learn” que cria cursos e materiais de treinamento para empresas.  Os grupos do Microsoft 365, com experiências colaborativas avançadas, são uma maneira fantástica de fornecer o conteúdo do curso e gravar exercícios entre os participantes de cursos online e presenciais.  Talvez você queira deixar os grupos do Microsoft 365 usados para cursos de treinamento facilmente identificados como cursos de treinamento, pois isso permite que outros desenvolvedores descubram seus grupos e criem experiências avançadas com base nos seus cursos de treinamento.

Para este cenário, este artigo lhe mostrará como:

1. Exibir definições de extensão de esquema disponíveis que você poderia usar.
2. Registrar uma definição de extensão de esquema direcionada a grupos de cursos de treinamento.
3. Criar um novo grupo com dados estendidos baseados na definição de extensão do esquema que você acabou de registrar.
4. Adicionar, atualizar ou remover dados personalizados em um grupo existente com base em uma definição de extensão de esquema.
5. Ler novamente um grupo e os dados de extensão.

>**Observação:** Este tópico mostra como criar e ler valores de extensão do esquema em um recurso **group** (etapas 3 a 5).  Os mesmos métodos são compatíveis também com os tipos de recurso **administrativeUnit**, **device**, **event**, **message**, **organization**, **post** e **user**.  Você pode executar operações semelhantes às solicitações do exemplo deste artigo em qualquer um desses recursos. Observe que **administrativeUnit** está disponível apenas no ponto de extremidade beta.

## <a name="1-view-available-schema-extensions"></a>1. Exibir extensões de esquema disponíveis
Em primeiro lugar, como desenvolvedor, talvez seja interessante localizar todas as outras definições de extensão de esquema que nosso aplicativo possa reutilizar.  Isso pode ser feito consultando o recurso **schemaExtension**.  
No exemplo abaixo, você consultará uma extensão de esquema específica por **id**.

Observe que a extensão retornada na resposta tem **Disponível** como o valor de **status**, que indica que qualquer aplicativo que tem permissão para os recursos na propriedade **targetTypes** pode usar e atualizar a extensão com alterações aditivas. Em geral, essa operação retorna quaisquer extensões de esquema que satisfaçam ao filtro especificado independentemente do **status**. Portanto, verifique o status da extensão antes de usá-la.


### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-get"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

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

Ao criar uma definição de extensão de esquema, você deve fornecer uma cadeia de caracteres para a propriedade **id**. Há duas maneiras de se fazer isso. O exemplo a seguir mostra o método preferencial, que usa um nome de domínio personalizado (`graphlearn.com`) que foi verificado com seu locatário. Concatene o nome de domínio verificado (`graphlearn`) com um nome para a extensão de esquema (`courses`) e atribua **id** com a cadeia de caracteres resultante, `graphlearn_courses`.  

Então especifique também uma descrição (para habilitar a capacidade de descoberta), tipos de destino (definindo a quais recursos essa extensão se aplica) e as propriedades personalizadas que compõem o esquema.  Neste exemplo, especifique as propriedades `courseId`, `courseName` e `courseType` personalizadas e seus tipos.

Veja um [exemplo de outra maneira de atribuir a **id** na solicitação](/graph/api/schemaextension-post-schemaextensions#request-2), que exige que você forneça apenas um nome de esquema.

Observe que, quando você cria uma extensão de esquema inicialmente, seu status é **InDevelopment**. Ao desenvolver a extensão, você pode mantê-la com esse status. Enquanto isso, apenas seu aplicativo que a criou pode atualizá-la com alterações aditivas ou excluí-la. Quando estiver pronto para compartilhar a extensão para uso por outros aplicativos, defina o **status** como **Disponível**.

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-createExtension"
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

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
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

## <a name="3-create-a-new-group-with-extended-data"></a>3. Criar um novo grupo com dados estendidos 
Criar um _novo_ grupo estendido com dados extras usando a definição de extensão de esquema `graphlearn_courses` que acabamos de registrar.  Este é um padrão ```POST``` para o recurso **group**, com a extensão de tipo complexo `graphlearn_courses` definida no corpo da solicitação.  A resposta não refletirá extensões de dados. Precisamos explicitamente usar a extensão ```$select``` por nome usando uma operação ```GET```.

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-createGroupWithExtension"
}-->
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
### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
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

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a>4. Adicionar, atualizar ou remover dados personalizados em um grupo existente
Você pode estender e adicionar dados personalizados a uma instância de grupo _existente_ a extensão de tipo complexo `graphlearn_courses` adicional no corpo de uma solicitação ```PATCH```.  

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-updateGroupWithExtension"
}-->
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

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

Se você quiser atualizar os valores dos dados de extensão, coloque todo o tipo complexo de extensão no corpo de uma solicitação ```PATCH``` (semelhante a adicionar dados personalizados a um recurso existente).

Você também pode remover dados personalizados adicionados a uma instância de recursos, definindo a propriedade de extensão correspondente como nulo. 

Para remover uma extensão de esquema de uma instância do recurso, defina o tipo complexo da extensão dessa instância como nulo.


## <a name="5-get-a-group-and-its-extension-data"></a>5. Obter um grupo e seus dados de extensão
Uma maneira conveniente de procurar um grupo (ou grupos) é usar `$filter` para corresponder a valores de propriedades de extensão específica, como um nome de extensão ou ID. 

Então, para obter os dados personalizados em um grupo, use `$select` para incluir a extensão de nome (neste caso, `graphlearn_courses`).

O exemplo a seguir procura o grupo que possui a extensão `graphlearn_courses` com um valor de propriedade `courseId` correspondente a `123` e obtém as propriedades do grupo **displayName**, **id** e **description** e os dados personalizados na extensão `graphlearn_courses`. (Na consulta em si, certifique-se de aplicar codificação de URL conforme necessário).

### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-getGroupSelectExtension"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
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

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](extensibility-overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](extensibility-open-users.md)
- [Domínios do Microsoft 365](/office365/servicedescriptions/office-365-platform-service-description/domains)
- [Adicionar e verificar um domínio para Microsoft 365](/microsoft-365/admin/setup/add-domain)
- [Tipo de recurso schemaExtension](/graph/api/resources/schemaextension)