# <a name="create-open-extension"></a>Criar extensão aberta

Crie uma extensão aberta (objeto [openTypeExtension](../resources/openTypeExtension.md)) e adicione propriedades personalizadas em uma instância nova ou existente de um recurso. 

## <a name="prerequisites"></a>Pré-requisitos

Uma das seguintes **permissões** é obrigatória para executar essa API, dependendo do recurso no qual você está criando a extensão.

|**Recurso com suporte**|**Permissão**|**Recurso com suporte**|**Permissão** |
|:-----|:-----|:-----|:-----|
| [device](../resources/device.md) | _Device.ReadWrite.All_ | [event](../resources/event.md) | _Calendars.ReadWrite_ |
| [group](../resources/group.md) | _Group.ReadWrite.All_ | [group event](../resources/event.md) | _Group.ReadWrite.All_ |
| [group post](../resources/post.md) | _Group.ReadWrite.All_ | [mensagem](../resources/message.md) | _Mail.ReadWrite_ |
| [organization](../resources/organization.md) | _Directory.AccessAsUser.All_ | [personal contact](../resources/contact.md) | _Contacts.ReadWrite_ |
| [user](../resources/user.md) | _Directory.AccessAsUser.All_ | | |


 
## <a name="http-request"></a>Solicitação HTTP

### <a name="create-an-extension-in-a-new-resource-instance"></a>Crie uma extensão em uma nova instância de recurso

Use a mesma solicitação REST conforme cria da instância. 

<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/events
POST /users/{id|userPrincipalName}/messages
POST /groups/{id}/events
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /users/{id|userPrincipalName}/contacts
```

>**Observação:** A sintaxe acima mostra algumas maneiras comuns de criar as instâncias de recursos com suporte. Todas as outras sintaxes POST que permitem criar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.

Confira a seção [Solicitar corpo](#request-body) sobre a inclusão de propriedades da nova instância do recurso _e a extensão_ no corpo da solicitação.

### <a name="create-an-extension-in-an-existing-resource-instance"></a>Crie uma extensão em uma instância de recurso existente

Identifique a instância do recurso na solicitação e faça um `POST` para a propriedade de navegação **extensions**.

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

>**Observação:** A sintaxe acima mostra algumas maneiras comuns de identificar uma instância do recurso, para criar uma extensão nele. Todas as outras sintaxes que permitem identificar essas instâncias de recursos dão suporte à criação de extensões abertas nelas de maneira semelhante.

Confira a seção [Solicitar corpo](#request-body) sobre como incluir _a extensão_ no corpo da solicitação.

## <a name="parameters"></a>Parâmetros
|**Parâmetro**|**Tipo**|**Descrição**|
|:-----|:-----|:-----|
|_Parâmetros de URL_|
|id|string|Um identificador exclusivo para um objeto na coleção correspondente. Obrigatório.|


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Valor |
|:---------------|:----------|
| Autorização | Bearer %token%|
| Content-Type | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um corpo JSON de uma [openTypeExtension](../resources/openTypeExtension.md), com os seguintes pares de nome/valor obrigatórios e dados personalizados adicionais. Os dados na carga JSON podem ser tipos primitivos ou matrizes de tipos primitivos.

| Name       | Valor |
|:---------------|:----------|
| @odata.type | Microsoft.Graph.OpenTypeExtension |
| extensionName | %unique_string% |

Ao criar uma extensão em uma _nova_ instância de recursos, além de novos objetos **openTypeExtension**, fornecem uma representação JSON das propriedades relevantes para criar uma instância de recurso deste tipo.

## <a name="response"></a>Resposta

#### <a name="response-code"></a>Código da resposta
Dependendo da operação, o código de resposta pode ser `201 Created` ou `202 Accepted`.

Ao criar uma extensão na mesma operação como criação de uma instância de recurso, uma operação bem-sucedida retorna o mesmo código de resposta que quando a operação é usada para criar apenas a instância de recurso sem a extensão. Consulte os tópicos correspondentes para criar a instância conforme listado [cima](#create-an-extension-in-a-new-resource-instance).

#### <a name="response-body"></a>Corpo da resposta
| Cenário       | Recurso  | Corpo da resposta |
|:---------------|:----------|:--------------|
| Criar uma extensão ao criar explicitamente uma _nova_ instância de recurso | [contact](../resources/contact.md), [event](../resources/event.md), [message](../resources/message.md) | Inclui a nova instância expandida com o objeto [openTypeExtension](../resources/openTypeExtension.md). |
| Criando uma extensão ao criar implicitamente uma instância de recursos | [postagem](../resources/post.md) | A resposta inclui somente um código de resposta, mas não um corpo de resposta. |
| Criar uma extensão em uma instância de recurso _existente_ | Todos os recursos com suporte | Inclui o objeto **openTypeExtension**. |
 


## <a name="example"></a>Exemplo
##### <a name="request-1"></a>Solicitação 1

O primeiro exemplo cria uma mensagem e uma extensão na mesma chamada. O corpo da solicitação inclui o seguinte:

- As propriedades **subject**, **body** e **toRecipients** típicas de uma nova mensagem. 
- E para a extensão:

  - O tipo `Microsoft.Graph.OpenTypeExtension`. 
  - O nome da extensão "Com.Contoso.Referral". 
  - Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e `dealValue`.  

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

##### <a name="response-1"></a>Resposta 1

Veja a seguir a resposta para o primeiro exemplo. O corpo da resposta inclui propriedades da nova mensagem e o seguinte para a nova extensão:

- A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`. 
- A propriedade padrão **extensionName** especificada na solicitação.
- Os dados personalizados especificados na solicitação, armazenados como 3 propriedades personalizadas.

Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
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

##### <a name="request-2"></a>Solicitação 2

O segundo exemplo cria uma extensão na mensagem especificada. O corpo da solicitação inclui o seguinte para essa extensão:

- O tipo `Microsoft.Graph.OpenTypeExtension`. 
- O nome da extensão "Com.Contoso.Referral".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.  

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

##### <a name="response-2"></a>Resposta 2

Veja a seguir a resposta para o segundo exemplo. O corpo da solicitação inclui o seguinte para a nova extensão:

- A propriedade padrão **extensionName**.
- A propriedade **id** com o nome totalmente qualificado de `Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral`. 
- Os dados personalizados a serem armazenados.  

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

##### <a name="request-3"></a>Solicitação 3

O terceiro exemplo cria uma extensão no evento de grupo especificado. O corpo da solicitação inclui o seguinte para essa extensão:

- O tipo `Microsoft.Graph.OpenTypeExtension`. 
- O nome da extensão "Com.Contoso.Deal".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `dealValue` e `expirationDate`.  

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

##### <a name="response-3"></a>Resposta 3

Veja a seguir a resposta da terceira solicitação de exemplo.

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

##### <a name="request-4"></a>Solicitação 4

O quarto exemplo cria uma extensão em uma nova postagem de grupo, usando a mesma chamada de ação **reply** para uma postagem de grupo existente. A ação **reply** cria uma nova postagem e uma nova extensão inserida nessa postagem. O corpo da solicitação inclui uma propriedade **post** que, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a nova extensão:

- O tipo `Microsoft.Graph.OpenTypeExtension`. 
- O nome da extensão "Com.Contoso.HR".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.

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

##### <a name="response-4"></a>Resposta 4

Veja a seguir a resposta do quarto exemplo. Criar uma extensão com êxito em uma nova postagem de grupo resulta apenas no código de resposta HTTP 202.

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

##### <a name="request-5"></a>Solicitação 5

O quinto exemplo cria uma extensão em uma nova postagem de grupo usando a mesma operação POST para criar uma conversa. A operação POST cria uma nova conversa, thread ou postagem e uma nova extensão inserida na postagem. O corpo da solicitação inclui as propriedades **Topic** e **Threads** e o objeto filho **post** para a nova conversa. O objeto **post**, por sua vez, contém o **corpo** da nova postagem e os seguintes dados para a extensão:

- O tipo `Microsoft.Graph.OpenTypeExtension`. 
- O nome da extensão "Com.Contoso.HR".
- Dados adicionais a serem armazenados como 3 propriedades personalizadas na carga JSON: `companyName`, `expirationDate` e a matriz de cadeias de caracteres `topPicks`.

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

##### <a name="response-5"></a>Resposta 5

Veja a seguir a resposta do quinto exemplo, que contém a nova conversa e uma ID de thread. Esse novo thread contém uma postagem criada automaticamente que, por sua vez, contém a nova extensão. 

Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

Para obter a nova extensão, primeiro [obtenha todas as postagens](../api/conversationthread_list_posts.md) desse thread. Inicialmente, deve haver somente uma. Em seguida, aplique a ID da postagem e o nome da extensão `Com.Contoso.Benefits` para [obter a extensão](../api/opentypeextension_get.md).

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
