---
title: Tipo de recurso teamworkHostedContent
description: Representa conteúdo rich hospedado por Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d53614b4d4f699890be7d244d78f7f1ec01890c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128176"
---
# <a name="teamworkhostedcontent-resource-type"></a>Tipo de recurso teamworkHostedContent

Namespace: microsoft.graph

Representa conteúdo rico como imagens e trechos de código em Microsoft Teams. Para conteúdo rico em [mensagens de canal e chat,](chatMessage.md)consulte [chatMessageHostedContent](chatMessageHostedContent.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentBytes|Binária|Somente gravação. Bytes para o conteúdo hospedado (como imagens).|
|contentType|String|Somente gravação. Tipo de conteúdo. sicj como image/png, image/jpg.|
|id|String|ID do conteúdo hospedado.|

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
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```
