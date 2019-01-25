---
title: tipo de recurso mencionam
description: Representa uma notificação para uma pessoa com base no endereço de email da pessoa.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523194"
---
# <a name="mention-resource-type"></a>tipo de recurso mencionam

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma notificação para uma pessoa com base no endereço de email da pessoa. Esse tipo de notificação é também conhecido como @ menções.

O recurso de [mensagem](../resources/message.md) suporta **mencionar**. Ela inclui uma propriedade **mentionsPreview** que indica se o usuário entrou no mencionada nessa instância da mensagem. Ele também inclui a propriedade de navegação **menções** , que oferece suporte para obter detalhes de um mencionam ou excluindo um mencionam nesse caso.

Ao criar uma mensagem, um aplicativo pode criar um mencionam na mesma `POST` solicitação, incluindo o mencionam na propriedade **menções** . Usando um `GET` solicitar com o `$filter` parâmetro de consulta, um aplicativo pode retornar todas as mensagens na caixa de correio do usuário conectado que mencionam o usuário. Uma `GET` solicitar com o `$expand` consulta parâmetro permite que o aplicativo expandir todas as menções em uma mensagem específica.

Esse mecanismo de deixar um aplicativo para definir e obter menções nas mensagens habilita notificações de leve, onde o usuário que está fazendo a mencionam pode permanecer no contexto existente (por exemplo, redigir um corpo de mensagem) enquanto o aplicativo define a propriedade subjacente **menções** . Mencionado pessoas facilmente podem descobrir se e onde eles são mencionados por meio de `GET` solicitações com o `$filter` ou `$expand` parâmetro de consulta.  

Por exemplo, no cliente de email do Outlook, quando um usuário digita `@` ao escrever uma mensagem, o Outlook permite que o usuário selecione ou digite um nome para concluir o @-mencionam. Outlook define a propriedade **menções** antes que ele cria e envia a mensagem ou evento. O Outlook também usa `GET` operações com `$filter` e `$expand` para permitir que o usuário entrou no procurar mensagens que mencionar o usuário, alertando o usuário para itens de ação ou discussões, que permite uma resposta mais rápida.


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
|aplicativo | String | O nome do aplicativo onde o mencionam é criado. Opcional. Não é usado e o padrão como nulo para a **mensagem**. |
|clientReference | String | Um identificador exclusivo que representa um pai da instância do recurso. Opcional. Não é usado e o padrão como nulo para a **mensagem**. |
|createdBy  | [emailAddress](../resources/emailaddress.md) | As informações de email do usuário que fez a mencionam. |
|createdDateTime  |DateTimeOffset |A data e hora em que o mencionam é criado no cliente. |
|deepLink | String | Um link profundo web ao contexto do mencionam na instância do recurso. Opcional. Não é usado e o padrão como nulo para a **mensagem**. |
|id | String| O identificador exclusivo de um mencionam em uma instância de recurso.|
|mencionado | [emailAddress](../resources/emailaddress.md) | As informações de email da pessoa mencionada. Obrigatório. |
|mentionText | String | Opcional. Não é usado e o padrão como nulo para a **mensagem**. Para obter as menções em uma mensagem, consulte a propriedade **bodyPreview** da mensagem em vez disso. |
|serverCreatedDateTime | DateTimeOffset | A data e hora em que o mencionam é criada no servidor. Opcional. Não é usado e o padrão como nulo para a **mensagem**. |

## <a name="relationships"></a>Relacionamento
Nenhum


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[POST](../api/user-sendmail.md#request-2) e enviar | Nenhum | Criar e enviar menções como parte de uma nova mensagem|
|[Post](../api/user-post-messages.md#request-2) para um novo rascunho | [mensagem](../resources/message.md) que contém um ou mais objetos **mencionar** . | Criar um rascunho de uma nova mensagem e incluir um ou mais objetos **mencionar** .|
|Mensagens de [obter](../api/user-list-messages.md#request-2) mencionar me | Coleção [message](../resources/message.md) | Obtenha todas as mensagens na caixa de correio do usuário conectado que contêm um **mencionar** deste usuário.|
|[Obtenha](../api/message-get.md#request-2) uma mensagem e seus menções | Coleção [message](../resources/message.md) | Obtenha uma mensagem e expanda os detalhes de cada **mencionar** na mensagem.|
|Excluir uma menção | Nenhum |Exclui a menção especificada na mensagem especificada na caixa de correio do usuário conectado. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
