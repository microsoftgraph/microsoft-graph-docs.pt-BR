---
title: Tipo de recurso teamworkHostedContent
description: Representa conteúdo rich hospedado pelo Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da0b157bab78867bd3309b4529afe8ef734f0144
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882310"
---
# <a name="teamworkhostedcontent-resource-type"></a>Tipo de recurso teamworkHostedContent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa conteúdo rico como imagens e trechos de código no Microsoft Teams. Para conteúdo rico em [mensagens de canal e chat,](chatMessage.md)consulte [chatMessageHostedContent](chatMessageHostedContent.md).

## <a name="methods"></a>Métodos

| Método                                            | Tipo de retorno                                       | Descrição                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [Obter bytes de ícone de aplicativo](../api/teamsappicon-get.md)     | [teamworkHostedContent](teamworkhostedcontent.md)                   | Obter os bytes do conteúdo hospedado com o backing de um ícone de aplicativo do Teams. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentBytes|Binária|Somente gravação. Bytes para o conteúdo hospedado (como imagens).|
|contentType|String|Somente gravação. Tipo de conteúdo, como image/png, image/jpg.|
|id|Cadeia de caracteres|ID do conteúdo hospedado.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```

