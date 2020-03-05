---
title: tipo de recurso menção
description: Representa uma notificação para uma pessoa com base no endereço de email da pessoa.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3780c4b01fc6dc81418034931f37e84d1e295b41
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522698"
---
# <a name="mention-resource-type"></a>tipo de recurso menção

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma notificação para uma pessoa com base no endereço de email da pessoa. Esse tipo de notificação também é conhecido como @ menciona.

O recurso [Message](../resources/message.md) dá suporte a **menção**. Ele inclui uma propriedade **mentionsPreview** que indica se o usuário conectado é mencionado nessa instância de mensagem. Ele também inclui a propriedade de navegação **menciona** , que oferece suporte a obter detalhes de uma menção ou excluir uma menção nessa instância.

Ao criar uma mensagem, um aplicativo pode criar uma menção na mesma `POST` solicitação, incluindo a menção na propriedade **menciona** . Usando uma `GET` solicitação com o `$filter` parâmetro de consulta, um aplicativo pode retornar todas as mensagens na caixa de correio do usuário conectado que mencionam o usuário. Uma `GET` solicitação com o `$expand` parâmetro de consulta permite que o aplicativo expanda todas as menção em uma mensagem específica.

Esse mecanismo de permitir que um aplicativo defina e receba mençãos em mensagens permite notificações leves, onde o usuário que faz a menção pode permanecer no contexto existente (como compor um corpo de mensagem) enquanto o aplicativo define a propriedade **mencionas** subjacentes. As pessoas mencionadas podem descobrir facilmente se e onde são mencionadas `GET` por meio de `$filter` solicitações `$expand` com o parâmetro ou consulta.  

Por exemplo, no cliente de email do Outlook, quando um usuário `@` digita uma mensagem, o Outlook permite que o usuário selecione ou insira um nome para concluir a menção @. O Outlook define a propriedade **menciona** antes de criar e enviar a mensagem ou o evento. O Outlook também `GET` usa operações `$filter` com `$expand` o e para permitir que o usuário conectado procure mensagens que mencionam o usuário, alertando o usuário sobre itens de ação ou discussões, o que permite uma resposta mais rápida.


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
|application | String | O nome do aplicativo em que a menção é criada. Opcional. Não usado e padronizado como nulo para a **mensagem**. |
|clientReference | String | Um identificador exclusivo que representa um pai da instância de recurso. Opcional. Não usado e padronizado como nulo para a **mensagem**. |
|createdBy  | [emailAddress](../resources/emailaddress.md) | As informações de email do usuário que fez a menção. |
|createdDateTime  |DateTimeOffset |A data e a hora em que a menção é criada no cliente. |
|deepLink | String | Um link profundo da Web para o contexto de menção na instância de recurso. Opcional. Não usado e padronizado como nulo para a **mensagem**. |
|id | String| O identificador exclusivo de uma menção em uma instância de recurso.|
|foi | [emailAddress](../resources/emailaddress.md) | As informações de email da pessoa mencionada. Obrigatório. |
|mentionText | String | Opcional. Não usado e padronizado como nulo para a **mensagem**. Para obter as menção em uma mensagem, confira a propriedade **bodyPreview** da mensagem. |
|serverCreatedDateTime | DateTimeOffset | A data e a hora em que a menção é criada no servidor. Opcional. Não usado e padronizado como nulo para a **mensagem**. |

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Post](../api/user-sendmail.md#request-2) e Send | Nenhum | Criar e enviar mençãos como parte de uma nova mensagem.|
|[Postar](../api/user-post-messages.md#request-2) em um novo rascunho | [mensagem](../resources/message.md) que contém um ou mais objetos de **menção** . | Crie um rascunho de uma nova mensagem e inclua um ou mais objetos de **menção** .|
|[Obter](../api/user-list-messages.md#request-2) mensagens mencionando-me | Coleção [message](../resources/message.md) | Obtenha todas as mensagens na caixa de correio do usuário conectado que contenham **menção** deste usuário.|
|[Obter](../api/message-get.md#request-2) uma mensagem e suas mencionações | Coleção [message](../resources/message.md) | Obtenha uma mensagem e expanda os detalhes de cada **menção** na mensagem.|
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
