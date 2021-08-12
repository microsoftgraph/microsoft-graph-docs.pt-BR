---
title: Tipo de recurso teamworkHostedContent
description: Representa conteúdo rich hospedado por Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7fca2d17db16e101edb22bd1ddfa31e4234e35ec6817f226209429f6cb97757a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189251"
---
# <a name="teamworkhostedcontent-resource-type"></a>Tipo de recurso teamworkHostedContent

Namespace: microsoft.graph

Representa conteúdo rico como imagens e trechos de código em Microsoft Teams. Para conteúdo rico em [mensagens de canal e chat,](chatMessage.md)consulte [chatMessageHostedContent](chatMessageHostedContent.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contentBytes|Binária|Somente gravação. Bytes para o conteúdo hospedado (como imagens).|
|contentType|String|Somente gravação. Tipo de conteúdo. sicj como image/png, image/jpg.|
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
