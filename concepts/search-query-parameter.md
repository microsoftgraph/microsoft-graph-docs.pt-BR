---
title: Use o parâmetro de consulta $search no Microsoft Graph
description: Microsoft Graph dá suporte ao parâmetro de consulta $search OData para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.
author: mumbi-o
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: ffb1a8024f0db673d14177a06f0635fce5a2a271
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436943"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a>Usar o parâmetro de consulta de pesquisa para corresponder a um critério de pesquisa

Além de [outros parâmetros de consulta OData](/graph/query-parameters), o Microsoft Graph dá suporte ao parâmetro de consulta `$search` para restringir os resultados de uma solicitação para corresponder a um critério de pesquisa.

O suporte para o parâmetro de consulta `$search` varia de acordo com a entidade, com alguns, como recursos do Microsoft Azure Active Directory que derivam de [directoryObject](/graph/api/resources/directoryobject), dando suporte a `$search` somente em [consultas avançadas](/graph/aad-advanced-queries).

> [!NOTE]
> O parâmetro de consulta `$search` não está disponível no momento nos locatários Azure AD B2C. 

## <a name="using-search-on-message-collections"></a>Usando $search em conjuntos de mensagens

Você pode pesquisar mensagens com base em um valor nas propriedades de mensagens específicas. Os resultados da pesquisa são classificados pela data e hora em que a mensagem foi enviada. Uma solicitação `$search` retorna até 1000 resultados.

Se você realizar uma pesquisa em mensagens e especificar apenas um valor sem as propriedades de mensagens específicas, a pesquisa será realizada nas propriedades de pesquisa padrão **from**, **subject** e **body**.

O exemplo a seguir retorna todas as mensagens na Caixa de Entrada do usuário que contenham "pizza" em qualquer uma das três propriedades de pesquisa padrão:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

Como alternativa, você pode pesquisar mensagens especificando os nomes de propriedade da mensagem na tabela a seguir, que são reconhecidos pela sintaxe da Linguagem de Consulta de Palavra-chave (KQL). Esses nomes de propriedades correspondem às propriedades definidas na entidade **mensagem** do Microsoft Graph. O Outlook e outros aplicativos do Microsoft 365 como o SharePoint são compatíveis com a sintaxe KQL, proporcionando a conveniência de um domínio de descoberta comum para seus repositórios de dados.

| Propriedades de emails pesquisáveis | Descrição                                                                                                                                                             | Exemplo                                                                                                                          |
| :------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| **attachment**            | Os nomes dos arquivos anexados a uma mensagem de email.                                                                                                                        | [OBTER][search-att-example] `../me/messages?$search="attachment:api-catalog.md"`                                                   |
| **bcc**                   | O campo **Cco** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.                                                                            | [OBTER][search-bcc-example] `../me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`                     |
| **body**                  | O corpo de uma mensagem de email.                                                                                                                                           | [OBTER][search-body-example] `../me/messages?$search="body:excitement"`                                                            |
| **cc**                    | O campo **Cc** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.                                                                             | [OBTER][search-cc-example] `../me/messages?$search="cc:danas"&$select=subject,ccRecipients`                                        |
| **from**                  | O remetente de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.                                                                                   | [OBTER][search-from-example] `../me/messages?$search="from:randiw"&$select=subject,from`                                           |
| **hasAttachment**         | Verdadeiro se uma mensagem de email contiver um anexo que não seja um anexo embutido, caso contrário, falso.                                                                      | [OBTER][search-from-example] `../me/messages?$search="hasAttachments:true"`                                                        |
| **importance**            | A prioridade de uma mensagem de email, que um remetente pode especificar ao enviar uma mensagem. Os valores possíveis são `low`, `medium` ou `high`.                              | [OBTER][search-imp-example] `../me/messages?$search="importance:high"&$select=subject,importance`                                  |
| **kind**                  | O tipo de mensagem. Os valores possíveis são `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` ou `voicemail`. | [OBTER][search-kind-example] `../me/messages?$search="kind:voicemail"`                                                             |
| **participants**          | Os campos **de**, **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.                                             | [OBTER][search-part-example] `../me/messages?$search="participants:danas"`                                                         |
| **received**              | A data em que uma mensagem de email foi recebida pelo destinatário.                                                                                                             | [OBTER][search-rcvd-example] `../me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`                       |
| **recipients**            | Os campos **para**, **Cc** e **Cco** de uma mensagem de email, especificados como um endereço SMTP, nome de exibição ou alias.                                                       | [OBTER][search-rcpts-example] `../me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients` |
| **sent**                  | A data em que uma mensagem de email foi enviada pelo remetente.                                                                                                                  | [OBTER][search-sent-example] `../me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`                               |
| **size**                  | O tamanho de um item em bytes.                                                                                                                                           | [OBTER][search-size-example] `../me/messages?$search="size:1..500000"`                                                             |
| **subject**               | O texto na linha de assunto de uma mensagem de email. .                                                                                                                     | [OBTER][search-sbj-example] `../me/messages?$search="subject:has"&$select=subject`                                                 |
| **to**                    | O campo **para** de uma mensagem de email, especificado como um endereço SMTP, nome de exibição ou alias.                                                                             | [OBTER][search-to-example]`.../me/messages?$search="to:randiw"&$select=subject,toRecipients`                                       |

Para saber mais sobre as propriedades de email pesquisáveis, KQL como a sintaxe, operadores com suporte e dicas de pesquisa, confira os seguintes artigos:

- [Propriedades pesquisáveis no Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).

- [Referência de sintaxe da Linguagem de Consulta de Palavra-chave (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [Propriedades da mensagem e operadores de pesquisa para a Descoberta eletrônica In-loco no Exchange 2016](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)

## <a name="using-search-on-person-collections"></a>Usando $search em conjuntos de pessoas

Você pode usar a [API de Pessoas](/graph/api/resources/person) do Microsoft Graph para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. A API de Pessoas é compatível com o parâmetro de consulta `$search`. Uma solicitação de `$search` retorna até 250 resultados.

As pesquisas de pessoas ocorrem nas propriedades **displayName** e **emailAddress** do recurso [person](/graph/api/resources/person).

A seguinte solicitação faz uma pesquisa por uma pessoa chamada "Clara Barbosa" nas propriedades **displayName** e **emailAddress** em todos os indivíduos no conjunto de **Pessoas** do usuário conectado. Como uma pessoa denominada "Clara Barbosa" é relevante para o usuário conectado, as informações para "Clara Barbosa" são retornadas.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

O exemplo a seguir mostra a resposta.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

Saiba mais sobre a API de Pessoas em [Obter informações sobre pessoas relevantes](./people-example.md#search-people).  

## <a name="using-search-on-directory-object-collections"></a>Como usar $search nos conjuntos de objetos do diretório

Os recursos do Microsoft Azure Active Directory e suas relações que derivam de [directoryObject](/graph/api/resources/directoryobject) dão suporte ao parâmetro de consulta `$search` somente em consultas avançadas. A implementação da pesquisa **não** suporta `contains`. Em vez disso, ele usa uma abordagem de geração de tokens que funciona extraindo palavras do valor da propriedade e da cadeia de caracteres de pesquisa usando espaços, números, maiúsculas e minúsculas diferentes, e símbolos conforme mostrado nos exemplos a seguir:

- **Espaços**: `hello world` => `hello`, `world`
- **Caixa diferente**⁽¹⁾: `HelloWorld` ou `helloWORLD` => `hello`, `world`
- **Símbolos**⁽²⁾: `hello.world` => `hello`, `.`,`world`, `helloworld`
- **Números**: `hello123world` => `hello`,`123`, `world`

⁽¹⁾ Atualmente, a tokenização só funciona quando a caixa está mudando de minúsculas para maiúsculas, portanto, `HELLOworld` é considerada um único token: `helloworld`, e `HelloWORld` tem dois tokens: `hello`, `world`.
⁽²⁾ A lógica de tokenização também combina palavras que são separadas apenas por símbolos; por exemplo, pesquisar por `helloworld` irá localizar `hello-world` e `hello.world`.

> [!NOTE]
>
> - Observação: após a geração de tokens, os tokens são combinados independentemente da capitalização original e são combinados em qualquer ordem. Por exemplo, displayName `李四(David Li)` corresponderá a cadeia de caracteres de pesquisa como `李四(David Li)`, `李四`, `David`, `Li`, `David)`, `(李四`, `Li 李`.
> - O suporte à pesquisa com token funciona apenas nos campos **displayName** e **descrição**. Qualquer campo do tipo Cadeia de Caracteres pode ser inserido em `$search`; campos diferentes de **displayName** e **descrição** assumem o comportamento padrão `$filter` `startswith`.

Por exemplo:
# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/?$search="displayName:OneVideo OR mail:onevideo"
```

Isso procura todos os grupos com nomes de exibição que têm tokens `one` e `video` ou emails que começam com `onevideo`.  

`$search` também pode ser usado junto com o `$filter`:
# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "search_filter_groups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"
```

procurar todos os grupos habilitados para email com nomes de exibição que se pareçam com "OneVideo".
Os resultados são restringidos com base em uma conjunção lógica (um “AND”) do parâmetro `$filter` e na consulta inteira no parâmetro `$search`.

A sintaxe da pesquisa segue as seguintes regras:

- Formato genérico: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.
- O número de cláusulas (clause) não é limitado. O uso de parênteses para a precedência também é suportado.
- A sintaxe para cada cláusula é: “\<property>:\<text to search>”.
- O nome da propriedade deve ser especificado na cláusula. Qualquer propriedade que possa ser usada em `$filter` também pode ser usada dentro de `$search`. Dependendo da propriedade, o comportamento de pesquisa será "search" ou "startsWith" se a pesquisa não tiver suporte na propriedade.
- A cláusula inteira deve ser declarada entre aspas duplas. Se ele contiver aspas duplas ou barra invertida, ele deverá ser escapado com uma barra invertida. Todos os outros caracteres especiais devem ser codificados em URL.
- Operadores lógicos `AND` e `OR` devem ser colocados fora das aspas duplas e devem estar em maiúsculas.

A tabela a seguir mostra alguns exemplos.

| Classe de objeto | Descrição                                            | Exemplo                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------ | ------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Usuário         | O caderno de endereços exibe o nome do usuário.                 | 
  [OBTER](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr"`                                                                                                                    |
| Usuário         | O caderno de endereços exibe o nome ou o email do usuário.         | 
  [OBTER](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr" OR "mail:Guthr"`                                                                          |
| Grupo        | O caderno de endereços exibe o nome ou a descrição de um grupo. | 
  [OBTER](https://developer.microsoft.com/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive"` |
| Grupo        | Nome de exibição do catálogo de endereços em um grupo habilitado para email.     | 
  [OBTER](https://developer.microsoft.com/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"`                                          |

Ambas as entradas da cadeia de caracteres fornecidas em `$search`, bem como as propriedades pesquisáveis, são divididas em partes por espaços, uso de maiúsculas/minúsculas e tipos de caracteres (números e caracteres especiais).

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

## <a name="see-also"></a>Confira também

- [Usar parâmetros de consulta para personalizar respostas](/graph/query-parameters)
- [Recursos avançados de consulta em objetos de diretório do Microsoft Azure Active Directory](/graph/aad-advanced-queries)
- [Limitações de parâmetro de consulta](known-issues.md#query-parameters)
