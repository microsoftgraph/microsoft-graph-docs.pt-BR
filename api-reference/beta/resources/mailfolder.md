---
title: tipo de recurso mailFolder
description: Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.
ms.openlocfilehash: 49fd4571e3ebe35e04e4da4276c1816829ebc599
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035815"
---
# <a name="mailfolder-resource-type"></a>tipo de recurso mailFolder

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder-delta.md).

**Nomes de pasta conhecido**

O Outlook cria determinadas pastas para usuários por padrão. Em vez de usar o valor de **id** de pasta correspondente, para sua conveniência, você pode usar os nomes de pasta conhecido da tabela abaixo ao acessar essas pastas. Por exemplo, você pode obter a pasta Rascunhos usando seu nome conhecido com a seguinte consulta.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Nomes conhecidos funcionam independentemente da localidade da caixa de correio do usuário, portanto, a consulta acima retornará sempre na pasta Rascunhos do usuário independentemente de como ele é chamado.

| Nome da pasta conhecido | Descrição |
|:-----------------------|:------------|
| arquivo morto | As mensagens de pasta de arquivo morto são enviadas ao usar o recurso de arquivamento One_Click nos clientes do Outlook com suporte. **Observação:** isso não é o mesmo que o recurso de caixa de correio de arquivamento do Exchange online. |
| desorganização | As mensagens de baixa prioridade de pasta desorganização são movidas para ao usar o recurso desorganização. |
| conflitos | A pasta que contém itens conflitantes na caixa de correio. |
| conversationhistory | A pasta onde o Skype salva conversas de mensagens Instantâneas (se Skype estiver configurada para fazê-lo). |
| deleteditems | Os itens da pasta são movidos para quando eles são excluídos. |
| rascunhos | A pasta que contém as mensagens não enviadas. |
| caixa de entrada | A pasta de caixa de entrada. |
| junkemail | A pasta de lixo eletrônico. |
| localfailures | A pasta que contém itens que existem no cliente local, mas não puderam ser carregados no servidor. |
| msgfolderroot | A pasta "Superior do armazenamento de informações". Essa pasta é a pasta pai para as pastas que são exibidos em clientes de email normal, como a caixa de entrada. |
| caixa de saída | A pasta caixa de saída. |
| recoverableitemsdeletions | A pasta que contém itens excluída: excluído da pasta Itens excluídos ou por pressionar shift + delete no Outlook. Essa pasta não é visível em qualquer cliente de email do Outlook, mas os usuários finais podem interagir com ele por meio do recurso de **Recuperar itens excluídos do servidor** do Outlook ou do Outlook na web. |
| agendado | A pasta que contém as mensagens que são agendadas reaparecem na caixa de entrada usando o recurso de agendamento no Outlook para iOS. |
| SearchFolders | A pasta pai para todas as pastas de pesquisa definido na caixa de correio do usuário. |
| itens enviados | A pasta Itens enviados. |
| serverfailures | A pasta que contém itens que existem no servidor, mas não pôde ser sincronizados no cliente local. |
| syncissues | A pasta que contém os logs de sincronização criados pelo Outlook. |

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
|[Obter mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |Leia as propriedades e os relacionamentos do objeto mailFolder.|
|[Criar MailFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| Crie uma nova mailFolder na atual postando na coleção childFolders.|
|[Listar childFolders](../api/mailfolder-list-childfolders.md) |Coleção [mailFolder](mailfolder.md)| Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.|
|[Criar Mensagem](../api/mailfolder-post-messages.md) |[message](message.md)| Crie uma nova mensagem na mailFolder atual postando na coleção de mensagens.|
|[Listar mensagens](../api/mailfolder-list-messages.md) |Coleção [message](message.md)| Obtenha todas as mensagens na caixa de correio do usuário conectado, ou em uma pasta especificada na caixa de correio.|
|[Update](../api/mailfolder-update.md) | [mailFolder](mailfolder.md)|Atualize o objeto mailFolder especificado. |
|[Delete](../api/mailfolder-delete.md) | Nenhuma |Exclua o objeto mailFolder especificado. |
|[copy](../api/mailfolder-copy.md)|[mailFolder](mailfolder.md)|Copie uma mailFolder e seu conteúdo para outra mailFolder.|
|[delta](../api/mailfolder-delta.md)|Coleção [mailFolder](mailfolder.md)|Obtenha um conjunto de pastas de email que foram adicionadas, excluídas ou removidas da caixa de correio do usuário.|
|[move](../api/mailfolder-move.md)|[mailFolder](mailfolder.md)|Mova uma mailFolder e seu conteúdo para outra mailFolder.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[mailFolder](mailfolder.md)  |Criar uma ou mais propriedades estendidas de valor único em uma mailFolder nova ou existente.   |
|[Obter mailFolder com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Obtenha mailFolders que contêm uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [mailFolder](mailfolder.md) | Criar uma ou mais propriedades estendidas de vários valores em uma mailFolder nova ou existente.  |
|[Obter mailFolder com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [mailFolder](mailfolder.md) | Obtenha uma mailFolder que contém uma propriedade estendida com vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|childFolderCount|Int32|O número de mailFolders filho imediatas na mailFolder atual.|
|displayName|String|O nome de exibição da mailFolder.|
|id|String|Identificador exclusivo do mailFolder.|
|parentFolderId|String|O identificador exclusivo de mailFolder do mailFolder pai.|
|totalItemCount|Int32|O número de itens na mailFolder.|
|unreadItemCount|Int32|O número de itens na mailFolder marcados como não lidos.|
|wellKnownName|String|O nome da pasta conhecido para a pasta. Os valores possíveis são listados acima. Essa propriedade só é definida para pastas padrão criadas pelo Outlook. Para outras pastas, essa propriedade é **null**.|

**Acessar contagens de itens de forma eficiente**

O `TotalItemCount` e `UnreadItemCount` propriedades de uma pasta permitem que você convenientemente calcular o número de itens de leitura na pasta.
Eles permitem evitar consultas semelhante ao seguinte que pode acarretar uma latência significativa:

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

Pastas de email no Outlook podem conter mais de um tipo de itens, por exemplo, a caixa de entrada pode conter itens que são diferentes dos itens de email da solicitação de reunião. `TotalItemCount`e `UnreadItemCount` incluir itens em uma pasta de email, independentemente de seus tipos de item.

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:-------------|:-----|:------------|
|childFolders|Coleção [MailFolder](mailfolder.md)|A coleção de pastas filho na mailFolder.|
|messageRules | Coleção [messageRule](messagerule.md) | A coleção de regras que se aplicam à pasta da Caixa de Entrada do usuário. |
|mensagens|Coleção [Message](message.md)|A coleção de mensagens na mailFolder.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mailFolder. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "childFolders",
    "messageRules",
    "messages",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailFolder"
}-->

```json
{
  "childFolderCount": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "parentFolderId": "string",
  "totalItemCount": 1024,
  "unreadItemCount": 1024,
  "wellKnownName": "string",
  "childFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "messageRules": [ { "@odata.type": "microsoft.graph.messageRule" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]
}
```

## <a name="see-also"></a>Confira também

- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
