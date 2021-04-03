---
title: Tipo de recurso chatMessageHostedContent
description: Um conteúdo hospedado em uma mensagem de chat
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 842ccdcad3f185eb64572c91ce5b82d673a1d43f
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582561"
---
# <a name="chatmessagehostedcontent-resource-type"></a>Tipo de recurso chatMessageHostedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conteúdo do Teams hospedado em uma mensagem de chat, como imagens ou trechos de código.
[Anexos de arquivo](chatmessageattachment.md) não são conteúdo hospedado; eles são armazenados no SharePoint ou no OneDrive.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar chatMessageHostedContent](../api/chatmessage-list-hostedcontents.md) | [coleção chatMessageHostedContent](chatmessagehostedcontent.md) | Recupere a lista de **chatMessageHostedContent** para uma mensagem. |
| [Obter chatMessageHostedContent](../api/chatmessagehostedcontent-get.md) | [chatMessageHostedContent](chatmessagehostedcontent.md) | Leia as propriedades e as relações de um **objeto chatMessageHostedContent.** |

## <a name="properties"></a>Propriedades

chatMessageHostedContent deriva do trabalho em [equipeHostedContent](teamworkhostedcontent.md)

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id            |String       | Somente leitura. Representa o identificador de conteúdo hospedado da mensagem de chat.|
|contentBytes  |Edm.Binary   | Somente gravação. Ao postar o conteúdo hospedado da nova mensagem de chat, representa os bytes da carga. Eles são representados como uma cadeia de caracteres base64Encoded.|
|contentType   |String       | Somente gravação. Ao postar conteúdo hospedado na nova mensagem de chat, representa o tipo de conteúdo, como image/png.|

### <a name="instance-attributes"></a>Atributos de instância

Atributos de instância são propriedades com comportamentos especiais.
Essas propriedades são temporárias e definem o comportamento que o serviço deve executar ou fornecer valores de propriedade de curto prazo, como uma URL de download para um item que expira.

| Nome da propriedade                     | Tipo   | Descrição
|:----------------------------------|:-------|:--------------------------------
| @microsoft.graph.temporaryId      | string | Somente gravação. Representa a temporaryId do conteúdo hospedado ao postar uma mensagem para se referir ao conteúdo hospedado no **recurso chatMessage** que está sendo enviado.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "keyProperty": "id"
}-->

```json
{
  "@microsoft.graph.temporaryId": "String (identifier)",
  "id": "String (identifier)",
  "contentBytes": "String (binary)",
  "contentType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


