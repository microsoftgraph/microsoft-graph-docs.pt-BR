---
title: tipo de recurso mailFolder
description: Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 7ce778093689d07522408954ea5b0423aea94168
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629501"
---
# <a name="mailfolder-resource-type"></a>tipo de recurso mailFolder

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma pasta de email na caixa de correio de um usuário, como Caixa de entrada e Rascunhos. As pastas de email podem conter mensagens, outros itens do Outlook e pastas de correio filho.

Esse recurso tem suporte para o uso da [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/mailfolder-delta.md).

**Nomes de pasta conhecidos**

O Outlook cria determinadas pastas para usuários por padrão. Em vez de usar a pasta correspondente com valor **id** para sua conveniência, você pode usar os nomes das pastas conhecidas na tabela abaixo ao acessar essas pastas. Por exemplo, você encontra a pasta de Rascunhos usando seu nome reconhecido com a seguinte consulta.

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/drafts
```

Nomes conhecidos funcionam independentemente da localidade da caixa de correio do usuário, então a consulta acima sempre retornará a pasta de Rascunhos do usuário independentemente de como será nomeada.

| Nome da pasta conhecida | Descrição |
|:-----------------------|:------------|
| arquivar | As mensagens da pasta arquivo morto são enviadas ao usar o recurso arquivar One_Click em clientes do Outlook que são compatíveis com ele. **Observação:** esse não é o mesmo recurso de Caixa de Correio de Arquivamento do Exchange online. |
| Email secundário | As mensagens de baixa prioridade da pasta de email secundário são movidas ao usar o recurso email secundário. |
| Conflitos | A pasta que contém itens conflitantes na caixa de correio. |
| conversationhistory | A pasta em que o Skype salva conversas de mensagens Instantâneas (se o Skype está configurado para fazer isso). |
| deleteditems | Os itens da pasta são movidos quando são excluídas. |
| rascunhos | A pasta que contém as mensagens não enviadas. |
| caixa de entrada | A pasta caixa de entrada. |
| junkemail | A pasta lixo eletrônico. |
| localfailures | A pasta que contém itens que existem no cliente local, mas não podem ser carregados para o servidor. |
| msgfolderroot | A pasta "Superior do repositório de informações". Esta pasta é a pasta pai das pastas que são exibidas em clientes de email normais, como a caixa de entrada. |
| Caixa de saída | A pasta caixa de saída. |
| recoverableitemsdeletions | A pasta que contém itens excluídos de modo reversível: excluído da pasta Itens excluídos ou ao pressionar shift + delete no Outlook. Esta pasta não está visível em qualquer cliente de email do Outlook, mas os usuários finais podem interagir com ela pelo recurso **Recuperar itens excluídos do servidor** no Outlook ou no Outlook na web. |
| agendado | A pasta que contém mensagens que estão agendadas para serem exibidas na caixa de entrada usando o recurso de cronograma do Outlook para iOS. |
| SearchFolders | A pasta pai para todas as pastas de pesquisa definida na caixa de correio do usuário. |
| sentitems | A pasta Itens enviados. |
| serverfailures | A pasta que contém itens que existem no servidor, mas não podem ser sincronizados para o cliente local. |
| syncissues | A pasta que contém os logs de sincronização criados pelo Outlook. |

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
|[Listar mailFolders](../api/user-list-mailfolders.md) | Coleção [mailFolder](mailfolder.md)|Obter todas as pastas de email na caixa de correio do usuário especificado, incluindo qualquer pasta de pesquisa de email.|
|[Obter mailFolder](../api/mailfolder-get.md) | [mailFolder](mailfolder.md) |Leia as propriedades e os relacionamentos do objeto mailFolder.|
|[Criar MailFolder](../api/user-post-mailfolders.md) |[mailFolder](mailfolder.md)| Crie uma nova pasta de email na pasta raiz da caixa de correio do usuário.|
|[Listar childFolders](../api/mailfolder-list-childfolders.md) |Coleção [mailFolder](mailfolder.md)| Obtenha a coleção de pastas sob a pasta especificada. Você pode usar o atalho `.../me/MailFolders` para obter a coleção de pastas de nível superior e navegar até outra pasta.|
|[Criar childFolder](../api/mailfolder-post-childfolders.md) |[mailFolder](mailfolder.md)| Crie uma nova mailFolder na atual postando na coleção childFolders.|
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
|id|String|Identificador exclusivo de mailFolder.|
|isHidden|Booliano|Indica se o mailFolder está oculto. Essa propriedade só pode ser definida ao criar a pasta. Encontre mais informações em [Pastas de email ocultas](#hidden-mail-folders).|
|parentFolderId|String|O identificador exclusivo de mailFolder do mailFolder pai.|
|totalItemCount|Int32|O número de itens na mailFolder.|
|unreadItemCount|Int32|O número de itens na mailFolder marcados como não lidos.|
|wellKnownName|Cadeia de caracteres|O nome da pasta conhecido para a pasta. Os valores possíveis estão listados acima. Essa propriedade só é definida para pastas padrão criadas por Outlook. Para outras pastas, essa propriedade é **nula**.|

**Acessar contagens de itens de forma eficiente**

As propriedades `TotalItemCount` e `UnreadItemCount` de uma pasta permitem convenientemente calcular o número de itens de leitura na pasta.
Eles permitem que você evite consultas semelhante à seguinte, que podem causar latência significativa:

```http
https://outlook.office.com/api/beta/me/folders/inbox/messages?$count=true&$filter=isread%20eq%20false
```

As pastas de email no Outlook podem conter mais de um tipo de item, por exemplo, a caixa de entrada pode conter itens que são diferentes de itens de email da solicitação de reunião. `TotalItemCount` e `UnreadItemCount` incluem itens em uma pasta de email independentemente seus tipos de item.

### <a name="hidden-mail-folders"></a>Pastas de email ocultas
O valor padrão da `isHidden` propriedade é `false` . Você pode definir **isHidden** apenas uma vez ao [criar o mailFolder](../api/user-post-mailfolders.md). Não é possível atualizar a propriedade usando uma operação PATCH. Para alterar a **propriedade isHidden** de uma pasta, exclua a pasta existente e crie uma nova com o valor desejado.

As pastas de email ocultas suportam todas as operações que são suportadas por uma pasta de email regular.

Por padrão, [listar mailFolders](../api/user-list-mailfolders.md) retorna apenas pastas de email que não estão ocultas. Para incluir pastas de email ocultas na resposta, use o parâmetro de consulta `includeHiddenFolders=true` . Em seguida, use a **propriedade isHidden** para identificar se uma pasta de email está oculta. 

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
  "isHidden": false,
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
<!--
{
  "type": "#page.annotation",
  "description": "mailFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


