---
title: Atualizar contato
description: Atualize as propriedades do objeto de contato.
author: kevinbellinger
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: bfd80a3b3fb465854f80479614437f8890d4948d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60990286"
---
# <a name="update-contact"></a>Atualizar contato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do objeto de contato.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Contacts.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Contacts.ReadWrite    |
|Aplicativo | Contacts.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
Um [contato](../resources/contact.md) do [contactFolder](../resources/contactfolder.md)padrão do usuário.
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
Um [contact](../resources/contact.md) da [contactFolder](../resources/contactfolder.md) de nível superior do usuário.
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
Um [contact](../resources/contact.md) incluso em uma pasta filha de uma [contactFolder](../resources/mailfolder.md).  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.
```http
PATCH /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|assistantName|String|O nome do assistente do contato.|
|birthday|DateTimeOffset|O aniversário do contato.|
|categories|String|As categorias associadas ao contato.|
|children|String||
|companyName|String|O nome da empresa do contato.|
|departamento|String|O departamento do contato.|
|displayName|String|O nome para exibição do contato. Observe que atualizações posteriores em outras propriedades podem fazer com que um valor gerado automaticamente sobrescreva o valor de displayName que você especificou. Para preservar a um valor preexistente, inclua-o como o displayName na operação atualizar.|
|emailAddresses|[Coleção typedEmailAddress](../resources/typedemailaddress.md)|Os endereços de email do contato.|
|fileAs|String|O nome com o qual o contato está arquivado.|
|gender |Cadeia de caracteres |O sexo do contato. |
|generation|String|A geração do contato.|
|givenName|String|O nome do contato.|
|imAddresses|String|Os endereços de mensagens instantâneas do contato.|
|initials|String|As iniciais do contato.|
|jobTitle|String|O cargo do contato.|
|manager|String|O nome do gerente do contato.
|middleName|String|O nome do meio do contato.|
|nickName|String|O apelido do contato.|
|officeLocation|String|O local do escritório do contato.|
|parentFolderId|String|A ID da pasta pai do contato.|
|personalNotes|String|As anotações do usuário sobre o contato.|
|telefones |Coleção [phone](../resources/phone.md) |Telefone números associados ao contato, por exemplo, telefone 1, celular e telefone comercial. |
|postalAddresses |[Coleção physicalAddress](../resources/physicaladdress.md) |Endereços associados ao contato, por exemplo, endereço residencial e endereço comercial. |
|profession|String|A profissão do contato.|
|spouseName|String|O nome do cônjuge/parceiro do contato.|
|surname|String|O sobrenome do contato.|
|title|String|O título do contato.|
|websites |Coleção [website](../resources/website.md)|Sites associados ao contato. |
|weddingAnniversary |Data |O aniversário de casamento do contato. |
|yomiCompanyName|String|O nome de empresa japonês fonético do contato. Essa propriedade é opcional.|
|yomiGivenName|String|O nome japonês fonético do contato. Essa propriedade é opcional.|
|yomiSurname|String|O sobrenome japonês fonético do contato. Essa propriedade é opcional.|

Como o **recurso de** contato dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância de `PATCH` contato existente. 

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [de](../resources/contact.md) contato atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
O exemplo a seguir atualiza o endereço de email pessoal do contato especificado.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-contact-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


