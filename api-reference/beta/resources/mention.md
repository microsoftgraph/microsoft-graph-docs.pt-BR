---
title: mencionar tipo de recurso
description: Representa uma notificação para uma pessoa com base no endereço de email da pessoa.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 23d4ac1d98a65e206a476768569cca89fb295a61
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844855"
---
# <a name="mention-resource-type"></a>mencionar tipo de recurso

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma notificação para uma pessoa com base no endereço de email da pessoa. Esse tipo de notificação também é conhecido como @menções.

O [recurso de](../resources/message.md) mensagem é compatível com **menção.** Ele inclui uma **propriedade mentionsPreview** que indica se o usuário assinado é mencionado nessa instância da mensagem. Ele também inclui a propriedade **de navegação de** menções, que oferece suporte para obter detalhes de uma menção ou excluir uma menção nessa instância.

Ao criar uma mensagem, um aplicativo pode criar uma menção na mesma solicitação incluindo a `POST` menção na propriedade **menções.** Usando uma solicitação com o parâmetro de consulta, um aplicativo pode retornar todas as mensagens na caixa de correio do usuário que menciona `GET` `$filter` o usuário. Uma `GET` solicitação com `$expand` o parâmetro de consulta permite que o aplicativo expanda todas as menções em uma mensagem específica.

Esse mecanismo de permitir que um aplicativo seja definido e receba menções em mensagens permite notificações leves, em que o usuário que faz a menção pode permanecer no contexto existente (como compor um corpo de mensagem) enquanto o aplicativo define a propriedade de menções **subjacentes.** As pessoas mencionadas podem facilmente descobrir se e onde são mencionadas por meio de `GET` solicitações com `$filter` o parâmetro `$expand` ou consulta.  

Por exemplo, no cliente de email do Outlook, quando um usuário digita enquanto escreve uma mensagem, o Outlook permite que o usuário selecione ou insira um nome para concluir `@` a @menção. O Outlook define **a propriedade de menções** antes de criar e enviar a mensagem ou o evento. Outlook also uses `GET` operations with and to let the `$filter` `$expand` signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|application | Cadeia de caracteres | O nome do aplicativo onde a menção foi criada. Opcional. Não usado e padrão como nulo para **mensagem**. |
|clientReference | Cadeia de caracteres | Um identificador exclusivo que representa um pai da instância do recurso. Opcional. Não usado e padrão como nulo para **mensagem**. |
|createdBy  | [emailAddress](../resources/emailaddress.md) | As informações de email do usuário que fez a menção. |
|createdDateTime  |DateTimeOffset |A data e a hora em que a menção é criada no cliente. |
|deepLink | Cadeia de caracteres | Um link da Web profundo para o contexto da menção na instância do recurso. Opcional. Não usado e padrão como nulo para **mensagem**. |
|id | Cadeia de caracteres| O identificador exclusivo de uma menção em uma instância de recurso.|
|mencionado | [emailAddress](../resources/emailaddress.md) | As informações de email da pessoa mencionada. Obrigatório. |
|mentionText | String | Opcional. Não usado e padrão como nulo para **mensagem**. Para obter as menções em uma mensagem, consulte a **propriedade bodyPreview** da mensagem. |
|serverCreatedDateTime | DateTimeOffset | A data e a hora em que a menção é criada no servidor. Opcional. Não usado e padrão como nulo para **mensagem**. |

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Postar](../api/user-sendmail.md#request-2) e enviar | Nenhum | Criar e enviar menções como parte de uma nova mensagem.|
|[Postar](../api/user-post-messages.md#request-2) em um novo rascunho | [que](../resources/message.md) contém um ou mais objetos **de menção.** | Crie um rascunho de uma nova mensagem e inclua um ou mais objetos **de menção.**|
|[Obter](../api/user-list-messages.md#request-2) mensagens mencionando-me | Coleção [message](../resources/message.md) | Obter todas as mensagens na caixa de correio do usuário que contêm **uma** menção a esse usuário.|
|[Obter](../api/message-get.md#example-2-get-all-mentions-in-a-specific-message) uma mensagem e suas menções | Coleção [message](../resources/message.md) | Obter uma mensagem e expandir os detalhes de **cada menção** na mensagem.|
|[Excluir](../api/message-delete.md#request-2) uma menção | Nenhum |Exclui a menção especificada na mensagem especificada na caixa de correio do usuário conectado. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


