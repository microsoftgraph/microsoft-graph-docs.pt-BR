# <a name="traverse-microsoft-graph"></a>Percorrer o Microsoft Graph

Além de usar a API do Microsoft Graph para ler e gravar dados, você pode usar diversos padrões de solicitação para desviar pelos recursos no Microsoft Graph. O documento de metadados também ajuda a entender o modelo de dados dos recursos e das relações no Microsoft Graph.

## <a name="microsoft-graph-api-metadata"></a>Metadados da API do Microsoft Graph

O documento de metadados ($metadata) é publicado na raiz do serviço. Você pode exibir o documento de serviço das versões 1.0 e beta da API Microsoft Graph com as URLs a seguir.

**Metadados da `v1.0` API do Microsoft Graph**
```
    https://graph.microsoft.com/v1.0/$metadata
```

**Metadados da `beta` API do Microsoft Graph**

```
    https://graph.microsoft.com/beta/$metadata
```

Os metadados permitem que você veja e entenda o modelo de dados do Microsoft Graph, incluindo os tipos de entidade, os tipos complexos e as enumerações que compõem os recursos representados nos pacotes de solicitação e resposta.

Você pode usar os metadados para compreender as relações entre entidades no Microsoft Graph e estabelecer URLs que navegam entre essas entidades.

Os nomes de recursos, parâmetros de consulta e parâmetros de ação da URL do caminho e os valores não diferenciam maiúsculas de minúsculas. No entanto, os valores que atribuir, as IDs de entidade e outros valores codificados na base 64 diferenciam maiúsculas de minúsculas.

## <a name="view-a-specific-resource-from-a-collection-by-id"></a>Exibir um recurso específico de uma coleção pela ID

Para exibir as informações sobre um usuário, você obtém a coleção de todos os usuários e usa uma solicitação GET HTTPS para chegar a um usuário específico pela ID do usuário. Para uma entidade `User`, você pode usar a propriedade `id` ou `userPrincipalName` como o identificador. A solicitação de exemplo a seguir usa o valor `userPrincipalName` como ID do usuário. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

Se tiver êxito, você obterá uma resposta 200 OK que contém a representação do recurso do usuário na carga, conforme mostrado.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```

## <a name="read-specific-properties-of-a-resource"></a>Ler propriedades específicas de um recurso
Para recuperar apenas os dados biográficos do usuário, conforme fornecido por ele na descrição _Sobre mim_, e suas habilidades, você pode adicionar o parâmetro de consulta [$select](query_parameters.md) à solicitação anterior, como mostrado no exemplo a seguir. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```
Aqui, em vez de todos os conjuntos de propriedade na entidade `user`, somente as propriedades básicas `aboutMe`, `displayName` e `skills` são retornadas.

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a>Ler propriedades específicas dos recursos em uma coleção
Além de ler propriedades específicas de um único recurso, você também pode aplicar o parâmetro de consulta [$select](query_parameters.md) semelhante a uma coleção para obter todos os recursos na coleção com apenas as propriedades específicas retornadas em cada um. Por exemplo, para consultar o nome dos itens na unidade do usuário conectado, você pode enviar a seguinte solicitação HTTPS GET.

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

A resposta bem-sucedida retorna um código de status 200 OK e uma carga que contém apenas os nomes dos arquivos compartilhados, conforme mostrado no exemplo abaixo.

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="traverse-from-one-resource-to-another-via-relationship"></a>Passar de um recurso para outro pela relação
Um gerente tem uma relação `directReports` com outros usuários diretamente subordinados a ele. Para consultar a lista de subordinados de um usuário, você pode usar a solicitação HTTPS GET a seguir para navegar para o destino pretendido via passagem de relação. 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

Da mesma forma, você pode seguir um relacionamento para navegar até os recursos relacionados. Por exemplo, a relação `user => messages` habilita a passagem de um usuário do Azure Active Directory (Azure AD) para um conjunto de mensagens de email do Outlook. O exemplo a seguir mostra como fazer isso em uma chamada à API REST.


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
A resposta bem-sucedida retorna o status 200 OK e uma carga, conforme mostrado.


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```
Você pode ver todas as relações em um determinado recurso indo para os metadados, localizando EntityType e examinando todas as NavigationProperties do EntityType.

## <a name="call-functions"></a>Funções de chamada
O Microsoft Graph também oferece suporte a _funções_ para manipular recursos de maneiras que não são apenas operações de criar, ler, atualizar e excluir (CRUD). Eles normalmente estão na forma de solicitações de HTTPS POST para receber argumentos para a função. Por exemplo, a seguinte função permite que o usuário conectado (`me`) envie uma mensagem de email.

```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

Você pode ver todas as funções que estão disponíveis nos metadados. Eles aparecem como Funções ou Ações.

## <a name="use-the-microsoft-graph-sdks"></a>Usar os SDKs do Microsoft Graph

Como o poder e a facilidade dos SDKs? Enquanto você sempre pode usar APIs REST para chamar o Microsoft Graph, também fornecemos SDKs para muitas plataformas populares. Para explorar os SDKs disponíveis, veja [Amostras de código e SDKs](https://graph.microsoft.io/en-us/code-samples-and-sdks).

## <a name="see-also"></a>Veja também

- [Usar a API do Microsoft Graph](use_the_api.md)
- [Obter tokens de autenticação](auth_overview.md)